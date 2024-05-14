==GPG==
	==Importing/Exporting Keys==
	gpg --armor --export soulsender > soulsender_pubkey.pgp
	gpg --import matze_pubk.pgp
	==Encrypting/Decrypting==
	gpg --encrypt message.txt
	==Listing Keys==
	gpg -k = List Public Keys
	gpg -K = List Secret Keys
	==Signing Keys==
	gpg --sign-key 123123123
	--armor (used for cross-platform)
	==Checksum==
	gpg --import KEYS
	gpg --verify downloaded_file.asc downloaded_file
	
==SSH==
	==Prepare Server==
	mkdir -p ~/.ssh
	chmod 700 ~/.ssh
	==Make New Keypair==
	ssh-keygen -t rsa
	==Copy Key To Server==
	ssh-copy-id -i ~/.ssh/id_rsa.pub user@server
	==Store Keys to Avoid ReAuth==
	ssh-agent $BASH
	ssh-add ~/.ssh/id_rsa
