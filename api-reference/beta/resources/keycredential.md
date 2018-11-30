---
title: keyCredential リソースの種類
description: アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。 アプリケーションと servicePrincipal のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。
ms.openlocfilehash: d4509360c0425c255566b9f77b9ecd96cf349dec
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27066794"
---
# <a name="keycredential-resource-type"></a><span data-ttu-id="378f1-104">keyCredential リソースの種類</span><span class="sxs-lookup"><span data-stu-id="378f1-104">keyCredential resource type</span></span>

> <span data-ttu-id="378f1-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="378f1-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="378f1-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="378f1-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="378f1-107">アプリケーションまたはサービス ・ プリンシパルに関連付けられているキーの資格情報が含まれています。</span><span class="sxs-lookup"><span data-stu-id="378f1-107">Contains a key credential associated with an application or a service principal.</span></span> <span data-ttu-id="378f1-108">[アプリケーション](application.md)と[servicePrincipal](serviceprincipal.md)のエンティティの**keyCredentials**プロパティは、 **keyCredential**のコレクションです。</span><span class="sxs-lookup"><span data-stu-id="378f1-108">The **keyCredentials** property of the [application](application.md) and [servicePrincipal](serviceprincipal.md) entities is a collection of **keyCredential**.</span></span>


## <a name="json-representation"></a><span data-ttu-id="378f1-109">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="378f1-109">JSON representation</span></span>

<span data-ttu-id="378f1-110">以下は、リソースの JSON 表記です</span><span class="sxs-lookup"><span data-stu-id="378f1-110">Here is a JSON representation of the resource</span></span>

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
## <a name="properties"></a><span data-ttu-id="378f1-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="378f1-111">Properties</span></span>
| <span data-ttu-id="378f1-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="378f1-112">Property</span></span>     | <span data-ttu-id="378f1-113">型</span><span class="sxs-lookup"><span data-stu-id="378f1-113">Type</span></span>   |<span data-ttu-id="378f1-114">説明</span><span class="sxs-lookup"><span data-stu-id="378f1-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="378f1-115">customKeyIdentifier</span><span class="sxs-lookup"><span data-stu-id="378f1-115">customKeyIdentifier</span></span>|<span data-ttu-id="378f1-116">バイナリ</span><span class="sxs-lookup"><span data-stu-id="378f1-116">Binary</span></span>| <span data-ttu-id="378f1-117">カスタム キー識別子</span><span class="sxs-lookup"><span data-stu-id="378f1-117">Custom key identifier</span></span> |
|<span data-ttu-id="378f1-118">endDateTime</span><span class="sxs-lookup"><span data-stu-id="378f1-118">endDateTime</span></span>|<span data-ttu-id="378f1-119">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="378f1-119">DateTimeOffset</span></span>|<span data-ttu-id="378f1-120">日付と、資格情報の有効期限が切れる。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="378f1-120">The date and time at which the credential expires.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="378f1-121">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="378f1-121">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="378f1-122">キー Id</span><span class="sxs-lookup"><span data-stu-id="378f1-122">keyId</span></span>|<span data-ttu-id="378f1-123">Guid</span><span class="sxs-lookup"><span data-stu-id="378f1-123">Guid</span></span>|<span data-ttu-id="378f1-124">キーの一意の識別子 (GUID)。</span><span class="sxs-lookup"><span data-stu-id="378f1-124">The unique identifier (GUID) for the key.</span></span>|
|<span data-ttu-id="378f1-125">startDateTime</span><span class="sxs-lookup"><span data-stu-id="378f1-125">startDateTime</span></span>|<span data-ttu-id="378f1-126">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="378f1-126">DateTimeOffset</span></span>|<span data-ttu-id="378f1-127">日付と時刻に、資格情報が有効になります。Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、UTC 時間に常に。</span><span class="sxs-lookup"><span data-stu-id="378f1-127">The date and time at which the credential becomes valid.The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="378f1-128">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="378f1-128">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="378f1-129">type</span><span class="sxs-lookup"><span data-stu-id="378f1-129">type</span></span>|<span data-ttu-id="378f1-130">String</span><span class="sxs-lookup"><span data-stu-id="378f1-130">String</span></span>|<span data-ttu-id="378f1-131">キーの資格情報の種類「対称」などです。</span><span class="sxs-lookup"><span data-stu-id="378f1-131">The type of key credential; for example, “Symmetric”.</span></span>|
|<span data-ttu-id="378f1-132">使用法</span><span class="sxs-lookup"><span data-stu-id="378f1-132">usage</span></span>|<span data-ttu-id="378f1-133">String</span><span class="sxs-lookup"><span data-stu-id="378f1-133">String</span></span>|<span data-ttu-id="378f1-134">キーが使われることができます; 目的を説明する文字列などの検証」です。</span><span class="sxs-lookup"><span data-stu-id="378f1-134">A string that describes the purpose for which the key can be used; for example, “Verify”.</span></span>|
|<span data-ttu-id="378f1-135">key</span><span class="sxs-lookup"><span data-stu-id="378f1-135">key</span></span>|<span data-ttu-id="378f1-136">Binary</span><span class="sxs-lookup"><span data-stu-id="378f1-136">Binary</span></span>|            |

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "keyCredential resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->