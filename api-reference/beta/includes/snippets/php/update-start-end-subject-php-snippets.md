---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;
use Microsoft\Graph\Beta\Generated\Models\OnlineMeeting;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new OnlineMeeting();
$requestBody->setStartDateTime(new \DateTime('2020-09-09T14:33:30.8546353-07:00'));
$requestBody->setEndDateTime(new \DateTime('2020-09-09T15:03:30.8566356-07:00'));
$requestBody->setSubject('Patch Meeting Subject');

$result = $graphServiceClient->me()->onlineMeetings()->byOnlineMeetingId('onlineMeeting-id')->patch($requestBody)->wait();

```