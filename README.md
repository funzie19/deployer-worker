# deployer-worker [![Build Status](https://travis-ci.org/funzie19/deployer-worker.svg?branch=master)](https://travis-ci.org/funzie19/deployer-worker)
Generates an Ansible deployer worker. This will be a user created on the remote machine to do all Ansible tasks.

=========

* Creates a user on the remote system
* Secures the user by removing the password
* Copies over the public key for the user
* Gives sudo access to user

Role Variables
--------------

deployer_username : Username to be created
	deployer_username: jkregloh

deployer_public_key : Public key of user

    deployer_public_key: |+
      ssh-rsa AAAAB3NzaC1yc2EAAAADAQABAAABAQC3u1bdRPITQygANTCxCI+CZptak8VgYnF21ddVCbW4s/EMrphyl8wpl17OU76euI4E/OJfMkrq9CI9hki9GeXm3fZip7AfcFy7qbUkHEXDElj8SmJD/kzt9K7Io/Hd/Le+d8k8ZZkEtqm7fQCH8e9PHMGU1f9l6WE29iHHHEy7ayRM2Hwb21bGaFTZ55VPo/Ks9w09kZAfQaNhM+LELs1Cwf282HAKnnjBB/xN1DuVsf/ZdR4Cj+/EnZX4+2VcK45od2mZtbN+nk+TesSp5cWGqwCyBFd0OmjNhg1DQmck3BcMTgT+3i9ZmVJi6uNrV4Jc99rlWMwWul86tvepB6Ep jkregloh@centos7.base

License
-------

MIT