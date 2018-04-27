# ansible-playbook -i ~/Downloads/hosts ~/Dropbox/code/scripts/ansible_single_cmd.yaml
- hosts: all
  ########################################################
  # ./hosts file contains:
  #
  # dzaratsian3.field.hortonworks.com
  # dzaratsian4.field.hortonworks.com
  # dzaratsian5.field.hortonworks.com 
  ########################################################
  
  remote_user: centos
  #become: yes
  #become_user: hdfs
  #become_method: su
  
  tasks:
  
  ########################################################
  #
  #   Current Python Version
  #
  ########################################################
  - name: Execute CMD
    #become: yes
    #become_user: root
    #become_method: sudo
    command: free -m
    register: result
  
  - debug: msg="{{ result }}"


##########################################################################################
#
# NOTES:
#
#   http://docs.ansible.com/ansible/latest/index.html
#
#   "command" is more secure than "shell". However, "shell" uses env variables. Some 
#   stream operations will also note work with "command", such as >, &, etc.
#
#
##########################################################################################

#ZEND
