# ansible

playbook: helloworld.yml

  play #1 (ec2): ec2    TAGS: []
    pattern: ['ec2']
    hosts (3):
      18.206.64.139
      3.87.48.181
      52.55.151.228

ansible-playbook helloworld.yml \
    --private-key ~/.ssh/EffectiveDevOpsAWS.pem \
    -e target=18.206.223.199 \
    --check

ansible-playbook helloworld.yml \
    --private-key ~/.ssh/EffectiveDevOpsAWS.pem \
    -e target=52.55.151.228 \
    --check