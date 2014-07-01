Vagrant.configure("2") do |config|
  config.vm.box = "dummy"

  config.vm.provider :aws do |aws, override|
    aws.access_key_id = ENV['AWS_ACCESS_KEY']
    aws.secret_access_key = ENV['AWS_SECRET_KEY']
    aws.keypair_name = "YOUR_KEYPAIR_NAME"

    aws.ami = "YOUR_AMI_ID"
    aws.instance_type = "t1.micro"
    aws.security_groups = ["YOUR_SECURITY_GROUP"]
    aws.tags = {
      'Name' => 'Dev Instance'
    }

    override.ssh.username = "ubuntu"
    override.ssh.private_key_path = "YOUR_PRIVATE_KEY_PATH"
  end
end