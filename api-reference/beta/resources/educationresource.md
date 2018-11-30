---
title: educationResource リソースの種類
description: システム内のすべてのリソース オブジェクトのスーパークラスです。 リソースは**割り当て**または**送信**される学習オブジェクトを表す、あるいはその両方に関連付けられています。
ms.openlocfilehash: b7e64a946992bb0b43c5bfe50e8d92b5f7176856
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27071885"
---
# <a name="educationresource-resource-type"></a><span data-ttu-id="2979c-104">educationResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2979c-104">educationResource resource type</span></span>

> <span data-ttu-id="2979c-105">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="2979c-105">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="2979c-106">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="2979c-106">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="2979c-107">システム内のすべてのリソース オブジェクトのスーパークラスです。</span><span class="sxs-lookup"><span data-stu-id="2979c-107">A superclass for all resource objects in the system.</span></span> <span data-ttu-id="2979c-108">リソースは**割り当て**または**送信**される学習オブジェクトを表す、あるいはその両方に関連付けられている割り当てられるまたは渡されました。</span><span class="sxs-lookup"><span data-stu-id="2979c-108">A resource is associated with an **Assignment** and/or **Submission**, which represents the learning object that is being handed out or handed in.</span></span> <span data-ttu-id="2979c-109">リソースを直接インスタンス化できません。使用されているリソースの種類を表すサブクラス化を行う必要があります。</span><span class="sxs-lookup"><span data-stu-id="2979c-109">You cannot instantiate a resource directly; you must make a subclass that will represent the type of resource being used.</span></span>

<span data-ttu-id="2979c-110">このリソースは、すべての種類のリソース間で共通のプロパティを格納します。</span><span class="sxs-lookup"><span data-stu-id="2979c-110">This resource stores the common properties across all resource types.</span></span>


## <a name="properties"></a><span data-ttu-id="2979c-111">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2979c-111">Properties</span></span>
| <span data-ttu-id="2979c-112">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2979c-112">Property</span></span>     | <span data-ttu-id="2979c-113">型</span><span class="sxs-lookup"><span data-stu-id="2979c-113">Type</span></span>   |<span data-ttu-id="2979c-114">説明</span><span class="sxs-lookup"><span data-stu-id="2979c-114">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="2979c-115">createdBy</span><span class="sxs-lookup"><span data-stu-id="2979c-115">createdBy</span></span>|[<span data-ttu-id="2979c-116">identitySet</span><span class="sxs-lookup"><span data-stu-id="2979c-116">identitySet</span></span>](identityset.md)|<span data-ttu-id="2979c-117">リソースを作成したとします。</span><span class="sxs-lookup"><span data-stu-id="2979c-117">Who created the resource.</span></span>|
|<span data-ttu-id="2979c-118">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2979c-118">createdDateTime</span></span>|<span data-ttu-id="2979c-119">リソースが作成された時点。</span><span class="sxs-lookup"><span data-stu-id="2979c-119">Moment in time when the resource was created.</span></span>  <span data-ttu-id="2979c-120">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2979c-120">DateTimeOffset</span></span>|<span data-ttu-id="2979c-p105">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、必ず UTC 時間です。たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2979c-p105">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time. For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|
|<span data-ttu-id="2979c-123">displayName</span><span class="sxs-lookup"><span data-stu-id="2979c-123">displayName</span></span>|<span data-ttu-id="2979c-124">String</span><span class="sxs-lookup"><span data-stu-id="2979c-124">String</span></span>|<span data-ttu-id="2979c-125">リソースの名前を表示します。</span><span class="sxs-lookup"><span data-stu-id="2979c-125">Display name of resource.</span></span>|
|<span data-ttu-id="2979c-126">lastModifiedBy</span><span class="sxs-lookup"><span data-stu-id="2979c-126">lastModifiedBy</span></span>|[<span data-ttu-id="2979c-127">identitySet</span><span class="sxs-lookup"><span data-stu-id="2979c-127">identitySet</span></span>](identityset.md)|<span data-ttu-id="2979c-128">ユーザーがリソースを変更する最後のユーザーです。</span><span class="sxs-lookup"><span data-stu-id="2979c-128">Who was the last user to modify the resource.</span></span>|
|<span data-ttu-id="2979c-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2979c-129">lastModifiedDateTime</span></span>|<span data-ttu-id="2979c-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2979c-130">DateTimeOffset</span></span>|<span data-ttu-id="2979c-131">リソースが最後に修正された瞬間です。</span><span class="sxs-lookup"><span data-stu-id="2979c-131">Moment in time when the resource was last modified.</span></span>  <span data-ttu-id="2979c-132">Timestamp 型は、ISO 8601 形式を使用して日付と時刻の情報を表し、常に UTC 時間です。</span><span class="sxs-lookup"><span data-stu-id="2979c-132">The Timestamp type represents date and time information using ISO 8601 format and is always in UTC time.</span></span> <span data-ttu-id="2979c-133">たとえば、2014 年 1 月 1 日午前 0 時 (UTC) は、次のようになります。`'2014-01-01T00:00:00Z'`</span><span class="sxs-lookup"><span data-stu-id="2979c-133">For example, midnight UTC on Jan 1, 2014 would look like this: `'2014-01-01T00:00:00Z'`</span></span>|

## <a name="json-representation"></a><span data-ttu-id="2979c-134">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2979c-134">JSON representation</span></span>

<span data-ttu-id="2979c-135">リソースの JSON 表記を次に示します。</span><span class="sxs-lookup"><span data-stu-id="2979c-135">The following is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "educationResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->