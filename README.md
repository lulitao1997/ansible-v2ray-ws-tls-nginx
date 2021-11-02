Role Name
=========

deploy v2ray + nginx, with the websocket + https setup

Requirements
------------

  - VPS with public ip address
  - domain with DNS records pointing to your VPS address

Role Variables
--------------

    v2ray_listen_port: 58600
    v2ray_uuid: <your uuid>
    v2ray_ws_path: /
    v2ray_cert_email: <your email address>
    v2ray_domain: <your domain>

Dependencies
------------

  - nginxinc.nginx
  - geerlingguy.certbot

Example Playbook
----------------

Including an example of how to use your role (for instance, with variables passed in as parameters) is always nice for users too:

    - hosts: servers

      vars:
        v2ray_domain: example.com
        v2ray_uuid: 00000-0000000000000000-0000
        v2ray_cert_email: webmaster@example.com

      roles:
        - ansible-v2ray-ws-tls-nginx

License
-------

BSD

