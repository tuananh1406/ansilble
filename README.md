### ANSIBLE AUTO DEPLOY HỆ THỐNG
## Các tags hiện  có
* install_gdnsd: Cài đặt gdnsd 2.3 lên server
* install_python: Cài đặt python 3.6.12 lên server
* install_logrotate: Cài đặt dnscap và setup logrotate trên server
# Ansible-playbook:
```shell
ansible-playbook -i hosts worker.yml -l <host_name> -t <tag_name>
```

        - Trong đó: 
                host_name: tên hoặc ip của server trong file host
                tag_name: tên tag cần chạy

- Bashscript đang dùng multipass để tạo server test
- Tự custom lại script nếu cần
# Bashscript:
```shell
chmod 755 run_install.sh
./run_install.sh <service>
```

        - Trong đó: 
                service: gdnsd hoặc python hoặc logrotate

- Bashscript đang dùng multipass để tạo server test
- Tự custom lại script nếu cần
