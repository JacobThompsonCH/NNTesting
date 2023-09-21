<!-- BEGIN_TF_DOCS -->


[36mrequirement.terraform[0m (~> 1.5.0)
[36mrequirement.aws[0m (~> 4.59.0)


[36mprovider.aws[0m (~> 4.59.0)


[36mmodule.fsx[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-fsx//,v0.0.6)
[36mmodule.fsx_quorum[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-fsx//,v0.0.6)
[36mmodule.fsx_quorum_sg[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-ec2-securitygroup//,v0.5.0)
[36mmodule.fsx_sg[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-ec2-securitygroup//,v0.5.0)
[36mmodule.fsx_software[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-fsx//,v0.0.6)
[36mmodule.fsx_software_sg[0m (git::git@gitlab.us.nelnet.biz:flyway/core/tf-consumable-modules/nn-tf-ec2-securitygroup//,v0.5.0)


[36mdata.aws_kms_key.default (data source)[0m (https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/kms_key)
[36mdata.aws_kms_key.default_key (data source)[0m (https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/kms_key)
[36mdata.aws_region.current (data source)[0m (https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/region)
[36mdata.aws_secretsmanager_secret.prodad (data source)[0m (https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/secretsmanager_secret)
[36mdata.aws_secretsmanager_secret_version.fsx_ad_join (data source)[0m (https://registry.terraform.io/providers/hashicorp/aws/latest/docs/data-sources/secretsmanager_secret_version)


[36minput.CI_PROJECT_NAME[0m (required)
[90mThe Gitlab Project name set from the pipeline variables[0m

[36minput.IAC_ORIGIN_VERSION[0m (required)
[90mGitlab project branch or tag for deployment[0m

[36minput.aliases[0m (required)
[90mAn array DNS alias names that you want to associate with the Amazon FSx file system[0m

[36minput.app_name[0m (required)
[90mn/a[0m

[36minput.aws_backup_tags[0m ({})
[90mAWS Backup tags[0m

[36minput.custom_rules[0m ({})
[90mn/a[0m

[36minput.data_classification[0m (null)
[90mData classification label per ADR-14 [0m

[36minput.default_key[0m (null)
[90mkms key alias, id, or arn of key for resource (ebs, s3, etc.) encryption[0m

[36minput.default_key_pair[0m (required)
[90mkey pair to be used for the ec2 instance[0m

[36minput.default_subnets[0m (null)
[90mList of all subnets[0m

[36minput.default_vpc_name[0m (required)
[90maws vpc[0m

[36minput.domain_name[0m ("nulsc.biz")
[90mNelnet domain[0m

[36minput.env[0m (required)
[90mshorter environmental team name[0m

[36minput.file_system_administrators_group[0m (required)
[90mThe name of the domain group whose members are granted administrative privileges for the file system[0m

[36minput.fs_name[0m (required)
[90mName prefix for FSx filesystem[0m

[36minput.fsx_quorum_sg_rules[0m ({})
[90mn/a[0m

[36minput.fsx_quorum_storage_capacity[0m (32)
[90mStorage capacity (GiB) of the sql quorum fsx file system[0m

[36minput.fsx_sg_rules[0m ({})
[90mn/a[0m

[36minput.fsx_software_sg_rules[0m ({})
[90mn/a[0m

[36minput.fsx_software_storage_capacity[0m (32)
[90mStorage capacity (GiB) of the sql software fsx file system[0m

[36minput.fsx_storage_capacity[0m (32)
[90mStorage capacity (GiB) of the sql backups fsx file system[0m

[36minput.fsx_tags[0m ({})
[90mTags used for FSx deployment[0m

[36minput.organizational_unit_distinguished_name[0m ("OU=WindowsServers,DC=nulsc,DC=biz")
[90mOU controlled by FSx service account[0m

[36minput.preferred_subnet_id[0m (null)
[90mID of primary private subnet for target fsx deployment.[0m

[36minput.quorum_fs_name[0m (required)
[90mName prefix for FSx filesystem[0m

[36minput.region[0m (required)
[90maws region[0m

[36minput.software_fs_name[0m (required)
[90mName prefix for FSx filesystem[0m

[36minput.subnet_ids[0m (required)
[90mA list of IDs for the subnets that the file system will be accessible from.[0m

[36minput.weekly_maintenance_start_time[0m ("0:01:00")
[90mPreferred start time to perform weekly maintenance, in the UTC time zone[0m


[36moutput.quorum_fsx[0m
[90mfsx details[0m

[36moutput.secret_server_fsx[0m
[90mfsx details[0m

[36moutput.software_fsx[0m
[90mfsx details[0m
<!-- END_TF_DOCS -->
