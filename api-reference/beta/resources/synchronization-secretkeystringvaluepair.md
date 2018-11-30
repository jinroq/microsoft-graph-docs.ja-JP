---
title: synchronizationSecretKeyStringValuePair リソースの種類
description: '1 つの秘密の値を表します。 '
ms.openlocfilehash: 31aa5d983a0117591d3be75939b2c881a9782e7c
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27073994"
---
# <a name="synchronizationsecretkeystringvaluepair-resource-type"></a><span data-ttu-id="4e95d-103">synchronizationSecretKeyStringValuePair リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4e95d-103">synchronizationSecretKeyStringValuePair resource type</span></span>

> <span data-ttu-id="4e95d-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="4e95d-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="4e95d-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4e95d-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="4e95d-106">1 つの秘密の値を表します。</span><span class="sxs-lookup"><span data-stu-id="4e95d-106">Represents a single secret value.</span></span> 

## <a name="properties"></a><span data-ttu-id="4e95d-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e95d-107">Properties</span></span>
| <span data-ttu-id="4e95d-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4e95d-108">Property</span></span>     | <span data-ttu-id="4e95d-109">型</span><span class="sxs-lookup"><span data-stu-id="4e95d-109">Type</span></span>   |<span data-ttu-id="4e95d-110">説明</span><span class="sxs-lookup"><span data-stu-id="4e95d-110">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4e95d-111">Key</span><span class="sxs-lookup"><span data-stu-id="4e95d-111">key</span></span>|<span data-ttu-id="4e95d-112">String</span><span class="sxs-lookup"><span data-stu-id="4e95d-112">String</span></span>| <span data-ttu-id="4e95d-113">使用可能な値: `None`、 `UserName`、 `Password`、 `SecretToken`、 `AppKey`、 `BaseAddress`、 `ClientIdentifier`、 `ClientSecret`、 `SingleSignOnType`、 `Sandbox`、 `Url`、 `Domain`、 `ConsumerKey`、 `ConsumerSecret`、 `TokenKey`、 `TokenExpiration`、 `Oauth2AccessToken`、 `Oauth2AccessTokenCreationTime`、 `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span><span class="sxs-lookup"><span data-stu-id="4e95d-113">Possible values are: `None`, `UserName`, `Password`, `SecretToken`, `AppKey`, `BaseAddress`, `ClientIdentifier`, `ClientSecret`, `SingleSignOnType`, `Sandbox`, `Url`, `Domain`, `ConsumerKey`, `ConsumerSecret`, `TokenKey`, `TokenExpiration`, `Oauth2AccessToken`, `Oauth2AccessTokenCreationTime`, `Oauth2RefreshToken`, `SyncAll`, `InstanceName`, `Oauth2ClientId`, `Oauth2ClientSecret`, `CompanyId`, `UpdateKeyOnSoftDelete`, `SynchronizationSchedule`, `SystemOfRecord`, `SandboxName`, `EnforceDomain`, `SyncNotificationSettings`, `Server`, `PerformInboundEntitlementGrants`, `HardDeletesEnabled`, `SyncAgentCompatibilityKey`, `SyncAgentADContainer`, `ValidateDomain`, `TestReferences`.</span></span>|
|<span data-ttu-id="4e95d-114">value</span><span class="sxs-lookup"><span data-stu-id="4e95d-114">value</span></span>|<span data-ttu-id="4e95d-115">文字列</span><span class="sxs-lookup"><span data-stu-id="4e95d-115">String</span></span>|<span data-ttu-id="4e95d-116">シークレットの値です。</span><span class="sxs-lookup"><span data-stu-id="4e95d-116">The value of the secret.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4e95d-117">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4e95d-117">JSON representation</span></span>

<span data-ttu-id="4e95d-118">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="4e95d-118">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "synchronizationSecretKeyStringValuePair resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->