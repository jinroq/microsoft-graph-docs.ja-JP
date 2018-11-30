---
title: passwordCredential リソースの種類
description: アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。 ServicePrincipal エンティティおよびアプリケーション エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。
ms.openlocfilehash: 79d3f76606533cf639f52ed22cd93f353e18e977
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066561"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="6bd8c-104">passwordCredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6bd8c-104">passwordCredential resource type</span></span>

> <span data-ttu-id="6bd8c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="6bd8c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="6bd8c-107">アプリケーションまたはサービスのプリンシパルに関連付けられているパスワード資格情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-107">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="6bd8c-108">[ServicePrincipal](serviceprincipal.md)エンティティおよび[アプリケーション](application.md)エンティティの**passwordCredentials**プロパティは、 **passwordCredential**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-108">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="6bd8c-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6bd8c-109">JSON representation</span></span>

<span data-ttu-id="6bd8c-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="6bd8c-110">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.passwordCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "secretText": "string",
  "hint": "string"
}

```
## <a name="properties"></a><span data-ttu-id="6bd8c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bd8c-111">Properties</span></span>
| <span data-ttu-id="6bd8c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6bd8c-112">Property</span></span>     | <span data-ttu-id="6bd8c-113">型</span><span class="sxs-lookup"><span data-stu-id="6bd8c-113">Type</span></span>   |<span data-ttu-id="6bd8c-114">説明</span><span class="sxs-lookup"><span data-stu-id="6bd8c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="6bd8c-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="6bd8c-115">customKeyIdentifier</span></span>|<span data-ttu-id="6bd8c-116">バイナリ</span><span class="sxs-lookup"><span data-stu-id="6bd8c-116">Binary</span></span>|            |
|<span data-ttu-id="6bd8c-117">endDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd8c-117">endDateTime</span></span>|<span data-ttu-id="6bd8c-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd8c-118">DateTimeOffset</span></span>|<span data-ttu-id="6bd8c-119">日付と時刻、パスワードの有効期限が切れます。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-119">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6bd8c-120">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6bd8c-120">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6bd8c-121">キー Id</span><span class="sxs-lookup"><span data-stu-id="6bd8c-121">keyId</span></span>|<span data-ttu-id="6bd8c-122">Guid</span><span class="sxs-lookup"><span data-stu-id="6bd8c-122">Guid</span></span>|            |
|<span data-ttu-id="6bd8c-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="6bd8c-123">startDateTime</span></span>|<span data-ttu-id="6bd8c-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6bd8c-124">DateTimeOffset</span></span>|<span data-ttu-id="6bd8c-125">日付と時刻にパスワードが有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-125">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="6bd8c-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="6bd8c-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="6bd8c-127">secretText</span><span class="sxs-lookup"><span data-stu-id="6bd8c-127">secretText</span></span>|<span data-ttu-id="6bd8c-128">String</span><span class="sxs-lookup"><span data-stu-id="6bd8c-128">String</span></span>| <span data-ttu-id="6bd8c-129">パスワードは 16 ~ 64 文字の長さである必要があります。</span><span class="sxs-lookup"><span data-stu-id="6bd8c-129">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="6bd8c-130">ヒント</span><span class="sxs-lookup"><span data-stu-id="6bd8c-130">hint</span></span>|<span data-ttu-id="6bd8c-131">String</span><span class="sxs-lookup"><span data-stu-id="6bd8c-131">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
