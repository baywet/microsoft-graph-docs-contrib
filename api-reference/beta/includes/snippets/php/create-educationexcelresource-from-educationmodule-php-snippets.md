---
description: "Automatically generated file. DO NOT MODIFY"
---

```php

<?php
use Microsoft\Graph\Beta\GraphServiceClient;
use Microsoft\Graph\Beta\Generated\Models\EducationModuleResource;
use Microsoft\Graph\Beta\Generated\Models\EducationExcelResource;


$graphServiceClient = new GraphServiceClient($tokenRequestContext, $scopes);

$requestBody = new EducationModuleResource();
$resource = new EducationExcelResource();
$resource->setOdataType('#microsoft.graph.educationExcelResource');
$resource->setDisplayName('test_excel_file.xlsx');
$additionalData = [
	'file' => [
		'odataid' => 'https://graph.microsoft.com/v1.0/drives/b!-Ik2sRPLDEWy_bR8l75jfeDcpXQcRKVOmcml10NQLQ1F2UVvTgEnTKi0GO59dbCL/items/01VANVJQZLIO353OYQOBCIFCJGKBSLB4DK',
	],
];
$resource->setAdditionalData($additionalData);
$requestBody->setResource($resource);

$result = $graphServiceClient->education()->classes()->byEducationClassId('educationClass-id')->modules()->byEducationModuleId('educationModule-id')->resources()->post($requestBody)->wait();

```