---
title: governanceSubject リソースの種類
description: 特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: a83825a147429c81b3e83b2f2fb384672d2f527e
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32506435"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="d38ac-103">governanceSubject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d38ac-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="d38ac-104">特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。</span><span class="sxs-lookup"><span data-stu-id="d38ac-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="d38ac-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d38ac-105">Properties</span></span>
| <span data-ttu-id="d38ac-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d38ac-106">Property</span></span>  | <span data-ttu-id="d38ac-107">型</span><span class="sxs-lookup"><span data-stu-id="d38ac-107">Type</span></span>       |<span data-ttu-id="d38ac-108">説明</span><span class="sxs-lookup"><span data-stu-id="d38ac-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="d38ac-109">id</span><span class="sxs-lookup"><span data-stu-id="d38ac-109">id</span></span>         |<span data-ttu-id="d38ac-110">String</span><span class="sxs-lookup"><span data-stu-id="d38ac-110">String</span></span>     | <span data-ttu-id="d38ac-111">件名の id。</span><span class="sxs-lookup"><span data-stu-id="d38ac-111">The id of the subject.</span></span>|
|<span data-ttu-id="d38ac-112">type</span><span class="sxs-lookup"><span data-stu-id="d38ac-112">type</span></span>       |<span data-ttu-id="d38ac-113">String</span><span class="sxs-lookup"><span data-stu-id="d38ac-113">String</span></span>     |<span data-ttu-id="d38ac-114">件名の種類。</span><span class="sxs-lookup"><span data-stu-id="d38ac-114">The type of the subject.</span></span> <span data-ttu-id="d38ac-115">この値は、 ``User``、 ``Group``、と``ServicePrincipal``することができます。</span><span class="sxs-lookup"><span data-stu-id="d38ac-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="d38ac-116">displayName</span><span class="sxs-lookup"><span data-stu-id="d38ac-116">displayName</span></span>|<span data-ttu-id="d38ac-117">String</span><span class="sxs-lookup"><span data-stu-id="d38ac-117">String</span></span>     |<span data-ttu-id="d38ac-118">件名の表示名。</span><span class="sxs-lookup"><span data-stu-id="d38ac-118">The display name of the subject.</span></span>|
|<span data-ttu-id="d38ac-119">email</span><span class="sxs-lookup"><span data-stu-id="d38ac-119">email</span></span>      |<span data-ttu-id="d38ac-120">String</span><span class="sxs-lookup"><span data-stu-id="d38ac-120">String</span></span>     |<span data-ttu-id="d38ac-121">ユーザーの件名の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="d38ac-121">The email address of the user subject.</span></span> <span data-ttu-id="d38ac-122">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="d38ac-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="d38ac-123">principalName</span><span class="sxs-lookup"><span data-stu-id="d38ac-123">principalName</span></span>|<span data-ttu-id="d38ac-124">String</span><span class="sxs-lookup"><span data-stu-id="d38ac-124">String</span></span>   |<span data-ttu-id="d38ac-125">ユーザーの件名のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="d38ac-125">The principal name of the user subject.</span></span> <span data-ttu-id="d38ac-126">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="d38ac-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="d38ac-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d38ac-127">Relationships</span></span>
<span data-ttu-id="d38ac-128">なし</span><span class="sxs-lookup"><span data-stu-id="d38ac-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="d38ac-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d38ac-129">JSON representation</span></span>

<span data-ttu-id="d38ac-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d38ac-130">Here is a JSON representation of the resource.</span></span>

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
