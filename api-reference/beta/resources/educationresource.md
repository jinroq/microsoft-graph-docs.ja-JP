---
title: educationResource リソースの種類
description: システム内のすべてのリソースオブジェクトのスーパークラス。 リソースが**割り当て**または**送信**(またはその両方) に関連付けられています。これは、指定された学習オブジェクトを表します。
localization_priority: Normal
author: mmast-msft
ms.prod: education
doc_type: resourcePageType
ms.openlocfilehash: 8dfb996c863e3b2aa5e319fcd2b4dc6dd246751a
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35972606"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="f4c6b-104">educationResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f4c6b-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f4c6b-105">システム内のすべてのリソースオブジェクトのスーパークラス。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="f4c6b-106">リソースが**割り当て**または**送信**に関連付けられています。これは、渡される、または渡される learning オブジェクトを表します。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="f4c6b-107">リソースを直接インスタンス化することはできません。使用されているリソースの種類を表すサブクラスを作成する必要があります。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="f4c6b-108">このリソースは、すべてのリソースの種類で共通のプロパティを格納します。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="f4c6b-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4c6b-109">Properties</span></span>
| <span data-ttu-id="f4c6b-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f4c6b-110">Property</span></span>     | <span data-ttu-id="f4c6b-111">型</span><span class="sxs-lookup"><span data-stu-id="f4c6b-111">Type</span></span>   |<span data-ttu-id="f4c6b-112">説明</span><span class="sxs-lookup"><span data-stu-id="f4c6b-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="f4c6b-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="f4c6b-113">createdBy</span></span>|[<span data-ttu-id="f4c6b-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="f4c6b-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="f4c6b-115">リソースの作成者。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-115">Who created the resource.</span></span>|
|<span data-ttu-id="f4c6b-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="f4c6b-116">createdDateTime</span></span>|<span data-ttu-id="f4c6b-117">リソースが作成された時点の時間。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="f4c6b-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4c6b-118">DateTimeOffset</span></span>|<span data-ttu-id="f4c6b-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4c6b-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="f4c6b-121">displayName</span><span class="sxs-lookup"><span data-stu-id="f4c6b-121">displayName</span></span>|<span data-ttu-id="f4c6b-122">String</span><span class="sxs-lookup"><span data-stu-id="f4c6b-122">String</span></span>|<span data-ttu-id="f4c6b-123">リソースの表示名。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-123">Display name of resource.</span></span>|
|<span data-ttu-id="f4c6b-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="f4c6b-124">lastModifiedBy</span></span>|[<span data-ttu-id="f4c6b-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="f4c6b-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="f4c6b-126">リソースを最後に変更したユーザー。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="f4c6b-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="f4c6b-127">lastModifiedDateTime</span></span>|<span data-ttu-id="f4c6b-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="f4c6b-128">DateTimeOffset</span></span>|<span data-ttu-id="f4c6b-129">リソースが最後に変更された時点の時刻。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="f4c6b-130">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="f4c6b-131">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="f4c6b-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="f4c6b-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f4c6b-132">JSON representation</span></span>

<span data-ttu-id="f4c6b-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="f4c6b-133">The following is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.educationResource"
}-->

```json
{
  "createdBy": {"@odata.type": "microsoft.graph.identitySet"},
  "createdDateTime": "String (timestamp)",
  "displayName": "String",
  "lastModifiedBy": {"@odata.type": "microsoft.graph.identitySet"},
  "lastModifiedDateTime": "String (timestamp)"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": []
}
-->
