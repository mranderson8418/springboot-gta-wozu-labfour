deploy:
  provider: elasticbeanstalk
  skip_cleanup: true
  region: us-east-2
  app: springboot-gta-wozu-labfour
  env: springbootgtawozulabfour-env
  zip_file: 'target/springboot-gta-wozu-labfour-0.0.1-SHAPSHOT.jar'
  bucket_name: elasticbeanstalk-us-east-2-010526258890
  bucket_path: springboot-gta-wozu-labfour
  on:
    branch: main
  access_key_id: $AWS_ACCESS_KEY_ID
  secret_access_key: $AWS_SECRET_ACCESS_KEY

  
  dpl_version: 1.10.16