---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;
use Microsoft\Graph\Beta\Generated\Models\Conversation;
use Microsoft\Graph\Beta\Generated\Models\ConversationThread;
use Microsoft\Graph\Beta\Generated\Models\Post;
use Microsoft\Graph\Beta\Generated\Models\ItemBody;
use Microsoft\Graph\Beta\Generated\Models\BodyType;
use Microsoft\Graph\Beta\Generated\Models\Extension;
use Microsoft\Graph\Beta\Generated\Models\OpenTypeExtension;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new Conversation();
$requestBody->setTopic('Does anyone have a second?');
$threadsConversationThread1 = new ConversationThread();
$postsPost1 = new Post();
$postsPost1Body = new ItemBody();
$postsPost1Body->setContentType(new BodyType('hTML'));
$postsPost1Body->setContent('This is urgent!');
$postsPost1->setBody($postsPost1Body);
$extensionsExtension1 = new OpenTypeExtension();
$extensionsExtension1->setOdataType('microsoft.graph.openTypeExtension');
$extensionsExtension1->setExtensionName('Com.Contoso.Benefits');
$additionalData = [
	'companyName' => 'Contoso',
	'expirationDate' => '2016-08-03T11:00:00.000Z',
	'topPicks' => [
'Employees only', 'Add spouse or guest', 'Add family', ],
];
$extensionsExtension1->setAdditionalData($additionalData);
$extensionsArray []= $extensionsExtension1;
$postsPost1->setExtensions($extensionsArray);

$postsArray []= $postsPost1;
$threadsConversationThread1->setPosts($postsArray);

$threadsArray []= $threadsConversationThread1;
$requestBody->setThreads($threadsArray);


$result = $graphServiceClient->groups()->byGroupId('group-id')->conversations()->post($requestBody)->wait();

```