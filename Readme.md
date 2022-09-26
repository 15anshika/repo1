| Parameter | Description |
| --- | --- |
| ***`s3_bucket`*** | The name of S3 Bucket to store the objects. |
| ***`region`*** | The AWS region where the service will be deployed. Default is **us-east-1** |
| ***`url_length`*** | The length of the key to be used for a short URL. Default is **8** |
| ***`hash_salt`*** | The salt so keys generated for short URL are unique only to you. A salt string can be between 6 and 32 characters providing decent randomization. [Reference](https://hashids.org/python/) |
| ***`expiration_days`*** | The number of days for short URLs before they expire. Default is **30** days |
| ***`is_custom_domain_available`*** | Set his to **true** if you would like to use a custom domain as an alias for the Cloudfront Distribution domain. If **true**, You should provide value for **dns_name** must be provided and Public Hosted Zone should be available for the Domain in Route53. Default value is **false**. |
| ***`dns_name`*** | The domain name to be used for URL shortener as an alias to Cloudfront distribution. |
| ***`env`*** | Env name for the service. Default is ***dev***. |
| ***`app_name`*** | Env name for the service. Default is ***dev***. |
| ***`is_enable_url_tracking`*** | To enable URL click tracking and storing stats in DynamoDB table. Default is: **short-url-tracking** |
| ***`insert_batch_size`*** | Insert operation batch size to DynamoDB table. Default is **10** |

