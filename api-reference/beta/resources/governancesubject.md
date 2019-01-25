---
title: governanceSubject リソースの種類
description: ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 3d24047b3af46136734de2486b041e67a34f3d83
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/24/2019
ms.locfileid: "29519165"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="58a80-103">governanceSubject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="58a80-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="58a80-104">ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。</span><span class="sxs-lookup"><span data-stu-id="58a80-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="58a80-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58a80-105">Properties</span></span>
| <span data-ttu-id="58a80-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="58a80-106">Property</span></span>  | <span data-ttu-id="58a80-107">型</span><span class="sxs-lookup"><span data-stu-id="58a80-107">Type</span></span>       |<span data-ttu-id="58a80-108">説明</span><span class="sxs-lookup"><span data-stu-id="58a80-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="58a80-109">id</span><span class="sxs-lookup"><span data-stu-id="58a80-109">id</span></span>         |<span data-ttu-id="58a80-110">String</span><span class="sxs-lookup"><span data-stu-id="58a80-110">String</span></span>     | <span data-ttu-id="58a80-111">サブジェクトの id です。</span><span class="sxs-lookup"><span data-stu-id="58a80-111">The id of the subject.</span></span>|
|<span data-ttu-id="58a80-112">type</span><span class="sxs-lookup"><span data-stu-id="58a80-112">type</span></span>       |<span data-ttu-id="58a80-113">String</span><span class="sxs-lookup"><span data-stu-id="58a80-113">String</span></span>     |<span data-ttu-id="58a80-114">サブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="58a80-114">The type of the subject.</span></span> <span data-ttu-id="58a80-115">値は、 ``User``、``Group``と``ServicePrincipal``。</span><span class="sxs-lookup"><span data-stu-id="58a80-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="58a80-116">displayName</span><span class="sxs-lookup"><span data-stu-id="58a80-116">displayName</span></span>|<span data-ttu-id="58a80-117">String</span><span class="sxs-lookup"><span data-stu-id="58a80-117">String</span></span>     |<span data-ttu-id="58a80-118">件名の表示名です。</span><span class="sxs-lookup"><span data-stu-id="58a80-118">The display name of the subject.</span></span>|
|<span data-ttu-id="58a80-119">email</span><span class="sxs-lookup"><span data-stu-id="58a80-119">email</span></span>      |<span data-ttu-id="58a80-120">String</span><span class="sxs-lookup"><span data-stu-id="58a80-120">String</span></span>     |<span data-ttu-id="58a80-121">ユーザーのサブジェクトの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="58a80-121">The email address of the user subject.</span></span> <span data-ttu-id="58a80-122">件名は、他の種類では、空であるか。</span><span class="sxs-lookup"><span data-stu-id="58a80-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="58a80-123">principalName</span><span class="sxs-lookup"><span data-stu-id="58a80-123">principalName</span></span>|<span data-ttu-id="58a80-124">String</span><span class="sxs-lookup"><span data-stu-id="58a80-124">String</span></span>   |<span data-ttu-id="58a80-125">ユーザーのサブジェクトのプリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="58a80-125">The principal name of the user subject.</span></span> <span data-ttu-id="58a80-126">件名は、他の種類では、空であるか。</span><span class="sxs-lookup"><span data-stu-id="58a80-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="58a80-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="58a80-127">Relationships</span></span>
<span data-ttu-id="58a80-128">なし</span><span class="sxs-lookup"><span data-stu-id="58a80-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="58a80-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="58a80-129">JSON representation</span></span>

<span data-ttu-id="58a80-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="58a80-130">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.governanceSubject"
}-->

```json
{
  "id": "String",  
  "displayName": "String",
  "email": "String",
  "principalName": "String",
  "type": "String"
}

```

<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!--
{
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": "",
  "suppressions": [
    "Error: /api-reference/beta/resources/governancesubject.md:\r\n      Exception processing links.\r\n    System.ArgumentException: Link Definition was null. Link text: !INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)\r\n      at ApiDoctor.Validation.DocFile.get_LinkDestinations()\r\n      at ApiDoctor.Validation.DocSet.ValidateLinks(Boolean includeWarnings, String[] relativePathForFiles, IssueLogger issues, Boolean requireFilenameCaseMatch, Boolean printOrphanedFiles)"
  ]
}
-->
