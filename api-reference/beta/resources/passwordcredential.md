---
title: passwordCredential リソースの種類
description: アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。 ServicePrincipal エンティティおよび application エンティティの**Passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 72b07c92456ba8c1b1681b8d00b1dc5d512bc355
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36009203"
---
# <a name="passwordcredential-resource-type"></a><span data-ttu-id="ce8a9-104">passwordCredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ce8a9-104">passwordCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="ce8a9-105">アプリケーションまたはサービスプリンシパルに関連付けられているパスワード資格情報を格納します。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-105">Contains a password credential associated with an application or a service principal.</span></span> <span data-ttu-id="ce8a9-106">[Serviceprincipal](serviceprincipal.md)エンティティおよび[Application](application.md)エンティティの**Passwordcredentials**プロパティは、 **passwordcredentials**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-106">The **passwordCredentials** property of the [servicePrincipal](serviceprincipal.md) entity and of the [application](application.md) entity is a collection of **passwordCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="ce8a9-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ce8a9-107">JSON representation</span></span>

<span data-ttu-id="ce8a9-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="ce8a9-108">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="ce8a9-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8a9-109">Properties</span></span>
| <span data-ttu-id="ce8a9-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ce8a9-110">Property</span></span>     | <span data-ttu-id="ce8a9-111">型</span><span class="sxs-lookup"><span data-stu-id="ce8a9-111">Type</span></span>   |<span data-ttu-id="ce8a9-112">説明</span><span class="sxs-lookup"><span data-stu-id="ce8a9-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ce8a9-113">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="ce8a9-113">customKeyIdentifier</span></span>|<span data-ttu-id="ce8a9-114">Binary</span><span class="sxs-lookup"><span data-stu-id="ce8a9-114">Binary</span></span>|            |
|<span data-ttu-id="ce8a9-115">endDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8a9-115">endDateTime</span></span>|<span data-ttu-id="ce8a9-116">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8a9-116">DateTimeOffset</span></span>|<span data-ttu-id="ce8a9-117">パスワードの有効期限が切れる日付と時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-117">The date and time at which the password expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce8a9-118">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ce8a9-118">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ce8a9-119">Id</span><span class="sxs-lookup"><span data-stu-id="ce8a9-119">keyId</span></span>|<span data-ttu-id="ce8a9-120">Guid</span><span class="sxs-lookup"><span data-stu-id="ce8a9-120">Guid</span></span>|            |
|<span data-ttu-id="ce8a9-121">startDateTime</span><span class="sxs-lookup"><span data-stu-id="ce8a9-121">startDateTime</span></span>|<span data-ttu-id="ce8a9-122">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="ce8a9-122">DateTimeOffset</span></span>|<span data-ttu-id="ce8a9-123">パスワードが有効になる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-123">The date and time at which the password becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="ce8a9-124">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="ce8a9-124">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="ce8a9-125">secretText</span><span class="sxs-lookup"><span data-stu-id="ce8a9-125">secretText</span></span>|<span data-ttu-id="ce8a9-126">String</span><span class="sxs-lookup"><span data-stu-id="ce8a9-126">String</span></span>| <span data-ttu-id="ce8a9-127">パスワードの長さは16-64 文字でなければなりません。</span><span class="sxs-lookup"><span data-stu-id="ce8a9-127">The passwords must be 16-64 characters in length</span></span> |
|<span data-ttu-id="ce8a9-128">hint</span><span class="sxs-lookup"><span data-stu-id="ce8a9-128">hint</span></span>|<span data-ttu-id="ce8a9-129">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ce8a9-129">String</span></span>|  |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "passwordCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
