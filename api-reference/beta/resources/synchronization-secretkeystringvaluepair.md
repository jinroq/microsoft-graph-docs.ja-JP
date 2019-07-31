---
title: synchronizationSecretKeyStringValuePair リソースの種類
description: '1つのシークレット値を表します。 '
localization_priority: Normal
doc_type: resourcePageType
author: davidmu1
ms.prod: microsoft-identity-platform
ms.openlocfilehash: ad3348cea31567cedfca9b2626c81383ab8c6b8f
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35964700"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="229f5-103">synchronizationSecretKeyStringValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="229f5-103">synchronizationSecretKeyStringValuePair resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="229f5-104">1つのシークレット値を表します。</span><span class="sxs-lookup"><span data-stu-id="229f5-104">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="229f5-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="229f5-105">Properties</span></span>
| <span data-ttu-id="229f5-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="229f5-106">Property</span></span>     | <span data-ttu-id="229f5-107">型</span><span class="sxs-lookup"><span data-stu-id="229f5-107">Type</span></span>   |<span data-ttu-id="229f5-108">説明</span><span class="sxs-lookup"><span data-stu-id="229f5-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="229f5-109">Key</span><span class="sxs-lookup"><span data-stu-id="229f5-109">key</span></span>|<span data-ttu-id="229f5-110">String</span><span class="sxs-lookup"><span data-stu-id="229f5-110">String</span></span>| <span data-ttu-id="229f5-111">可能な値: `None`、 `UserName` `Password` `SecretToken` `AppKey` `BaseAddress` `ClientIdentifier` `ClientSecret` `SingleSignOnType` `Sandbox` `Url` `Domain`、、、、、、、、、、、、 `ConsumerKey` `ConsumerSecret` `TokenKey` `TokenExpiration` `Oauth2AccessToken` `Oauth2AccessTokenCreationTime` `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="229f5-111">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="229f5-112">value</span><span class="sxs-lookup"><span data-stu-id="229f5-112">value</span></span>|<span data-ttu-id="229f5-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="229f5-113">String</span></span>|<span data-ttu-id="229f5-114">シークレットの値。</span><span class="sxs-lookup"><span data-stu-id="229f5-114">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="229f5-115">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="229f5-115">JSON representation</span></span>

<span data-ttu-id="229f5-116">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="229f5-116">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.synchronizationSecretKeyStringValuePair"
}-->

```json
{
  "key": "String",
  "value": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
