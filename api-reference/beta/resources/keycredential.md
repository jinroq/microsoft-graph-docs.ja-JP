---
title: keycredential リソースの種類
description: アプリケーションまたはサービスプリンシパルに関連付けられているキーの資格情報を含みます。 application エンティティおよび serviceprincipal エンティティの**keycredentials**プロパティは**keycredentials**のコレクションです。
localization_priority: Normal
ms.openlocfilehash: 312821a91bdbb1ad15e136d2b7fc8f9184df4eac
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33345387"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="9f00f-104">keycredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="9f00f-104">keyCredential resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="9f00f-105">アプリケーションまたはサービスプリンシパルに関連付けられているキーの資格情報を含みます。</span><span class="sxs-lookup"><span data-stu-id="9f00f-105">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="9f00f-106">[application](application.md)エンティティおよび[serviceprincipal](serviceprincipal.md)エンティティの**keycredentials**プロパティは**keycredentials**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="9f00f-106">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="9f00f-107">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="9f00f-107">JSON representation</span></span>

<span data-ttu-id="9f00f-108">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="9f00f-108">Here is a JSON representation of the resource</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.keyCredential"
}-->

```json
{
  "customKeyIdentifier": "binary",
  "endDateTime": "String (timestamp)",
  "keyId": "guid",
  "startDateTime": "String (timestamp)",
  "type": "string",
  "usage": "string",
  "key": "binary"
}

```
## <a name="properties"></a><span data-ttu-id="9f00f-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f00f-109">Properties</span></span>
| <span data-ttu-id="9f00f-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="9f00f-110">Property</span></span>     | <span data-ttu-id="9f00f-111">型</span><span class="sxs-lookup"><span data-stu-id="9f00f-111">Type</span></span>   |<span data-ttu-id="9f00f-112">説明</span><span class="sxs-lookup"><span data-stu-id="9f00f-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="9f00f-113">customkeyidentifier</span><span class="sxs-lookup"><span data-stu-id="9f00f-113">customKeyIdentifier</span></span>|<span data-ttu-id="9f00f-114">Binary</span><span class="sxs-lookup"><span data-stu-id="9f00f-114">Binary</span></span>| <span data-ttu-id="9f00f-115">カスタムキー識別子</span><span class="sxs-lookup"><span data-stu-id="9f00f-115">Custom key identifier</span></span> |
|<span data-ttu-id="9f00f-116">endDateTime</span><span class="sxs-lookup"><span data-stu-id="9f00f-116">endDateTime</span></span>|<span data-ttu-id="9f00f-117">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f00f-117">DateTimeOffset</span></span>|<span data-ttu-id="9f00f-118">資格情報の有効期限が切れる日付と時刻。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9f00f-118">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9f00f-119">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9f00f-119">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9f00f-120">id</span><span class="sxs-lookup"><span data-stu-id="9f00f-120">keyId</span></span>|<span data-ttu-id="9f00f-121">Guid</span><span class="sxs-lookup"><span data-stu-id="9f00f-121">Guid</span></span>|<span data-ttu-id="9f00f-122">キーの一意識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="9f00f-122">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="9f00f-123">startDateTime</span><span class="sxs-lookup"><span data-stu-id="9f00f-123">startDateTime</span></span>|<span data-ttu-id="9f00f-124">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="9f00f-124">DateTimeOffset</span></span>|<span data-ttu-id="9f00f-125">資格情報が有効になる日時。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="9f00f-125">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="9f00f-126">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="9f00f-126">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="9f00f-127">type</span><span class="sxs-lookup"><span data-stu-id="9f00f-127">type</span></span>|<span data-ttu-id="9f00f-128">String</span><span class="sxs-lookup"><span data-stu-id="9f00f-128">String</span></span>|<span data-ttu-id="9f00f-129">キーの資格情報の種類。たとえば、"Symmetric" となります。</span><span class="sxs-lookup"><span data-stu-id="9f00f-129">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="9f00f-130">上</span><span class="sxs-lookup"><span data-stu-id="9f00f-130">usage</span></span>|<span data-ttu-id="9f00f-131">String</span><span class="sxs-lookup"><span data-stu-id="9f00f-131">String</span></span>|<span data-ttu-id="9f00f-132">キーを使用できる目的を記述する文字列。たとえば、"Verify" とします。</span><span class="sxs-lookup"><span data-stu-id="9f00f-132">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="9f00f-133">key</span><span class="sxs-lookup"><span data-stu-id="9f00f-133">key</span></span>|<span data-ttu-id="9f00f-134">Binary</span><span class="sxs-lookup"><span data-stu-id="9f00f-134">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
