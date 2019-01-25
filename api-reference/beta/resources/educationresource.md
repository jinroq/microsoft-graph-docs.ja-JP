---
title: educationResource リソースの種類
description: システム内のすべてのリソース オブジェクトのスーパークラスです。 リソースは**割り当て**または**送信**される学習オブジェクトを表す、あるいはその両方に関連付けられています。
localization_priority: Normal
author: mmast-msft
ms.prod: education
ms.openlocfilehash: 87b19f849e24f1780a1d13c7aa1b3eb83543fdec
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29523219"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="c31b5-104">educationResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="c31b5-104">educationResource resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="c31b5-105">システム内のすべてのリソース オブジェクトのスーパークラスです。</span><span class="sxs-lookup"><span data-stu-id="c31b5-105">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="c31b5-106">リソースは**割り当て**または**送信**される学習オブジェクトを表す、あるいはその両方に関連付けられている割り当てられるまたは渡されました。</span><span class="sxs-lookup"><span data-stu-id="c31b5-106">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="c31b5-107">リソースを直接インスタンス化できません。使用されているリソースの種類を表すサブクラス化を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="c31b5-107">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="c31b5-108">このリソースは、すべての種類のリソース間で共通のプロパティを格納します。</span><span class="sxs-lookup"><span data-stu-id="c31b5-108">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="c31b5-109">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c31b5-109">Properties</span></span>
| <span data-ttu-id="c31b5-110">プロパティ</span><span class="sxs-lookup"><span data-stu-id="c31b5-110">Property</span></span>     | <span data-ttu-id="c31b5-111">型</span><span class="sxs-lookup"><span data-stu-id="c31b5-111">Type</span></span>   |<span data-ttu-id="c31b5-112">説明</span><span class="sxs-lookup"><span data-stu-id="c31b5-112">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="c31b5-113">createdBy</span><span class="sxs-lookup"><span data-stu-id="c31b5-113">createdBy</span></span>|[<span data-ttu-id="c31b5-114">identitySet</span><span class="sxs-lookup"><span data-stu-id="c31b5-114">identitySet</span></span>](identityset.md)|<span data-ttu-id="c31b5-115">リソースを作成したとします。</span><span class="sxs-lookup"><span data-stu-id="c31b5-115">Who created the resource.</span></span>|
|<span data-ttu-id="c31b5-116">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="c31b5-116">createdDateTime</span></span>|<span data-ttu-id="c31b5-117">リソースが作成された時点。</span><span class="sxs-lookup"><span data-stu-id="c31b5-117">Moment in time when the resource was created.</span></span>  <span data-ttu-id="c31b5-118">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c31b5-118">DateTimeOffset</span></span>|<span data-ttu-id="c31b5-p104">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c31b5-p104">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="c31b5-121">displayName</span><span class="sxs-lookup"><span data-stu-id="c31b5-121">displayName</span></span>|<span data-ttu-id="c31b5-122">String</span><span class="sxs-lookup"><span data-stu-id="c31b5-122">String</span></span>|<span data-ttu-id="c31b5-123">リソースの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="c31b5-123">Display name of resource.</span></span>|
|<span data-ttu-id="c31b5-124">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="c31b5-124">lastModifiedBy</span></span>|[<span data-ttu-id="c31b5-125">identitySet</span><span class="sxs-lookup"><span data-stu-id="c31b5-125">identitySet</span></span>](identityset.md)|<span data-ttu-id="c31b5-126">ユーザーがリソースを変更する最後のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="c31b5-126">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="c31b5-127">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="c31b5-127">lastModifiedDateTime</span></span>|<span data-ttu-id="c31b5-128">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="c31b5-128">DateTimeOffset</span></span>|<span data-ttu-id="c31b5-129">リソースが最後に修正された瞬間です。</span><span class="sxs-lookup"><span data-stu-id="c31b5-129">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="c31b5-130">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="c31b5-130">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="c31b5-131">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="c31b5-131">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="c31b5-132">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="c31b5-132">JSON representation</span></span>

<span data-ttu-id="c31b5-133">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="c31b5-133">The following is a JSON representation of the resource.</span></span>

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
  "suppressions": [
    "Error: /api-reference/beta/resources/educationresource.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
