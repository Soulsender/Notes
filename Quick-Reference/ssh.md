--Generate/Copy keys--
ssh-keygen
ssh-copy-id user@ip

--No Copy Command--
cat ~/.ssh/id_rsa.pub | ssh username@remote_host "mkdir -p ~/.ssh && cat >> ~/.ssh/authorized_keys"
