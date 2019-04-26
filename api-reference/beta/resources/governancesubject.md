---
title: governanceSubject リソースの種類
description: 特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。
localization_priority: Normal
ms.openlocfilehash: 5ad4b30abaec66b8ad35835795848645ddd9f17b
ms.sourcegitcommit: 014eb3944306948edbb6560dbe689816a168c4f7
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/26/2019
ms.locfileid: "33333693"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="4b986-103">governanceSubject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4b986-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="4b986-104">特権 id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。</span><span class="sxs-lookup"><span data-stu-id="4b986-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="4b986-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b986-105">Properties</span></span>
| <span data-ttu-id="4b986-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4b986-106">Property</span></span>  | <span data-ttu-id="4b986-107">型</span><span class="sxs-lookup"><span data-stu-id="4b986-107">Type</span></span>       |<span data-ttu-id="4b986-108">説明</span><span class="sxs-lookup"><span data-stu-id="4b986-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="4b986-109">id</span><span class="sxs-lookup"><span data-stu-id="4b986-109">id</span></span>         |<span data-ttu-id="4b986-110">String</span><span class="sxs-lookup"><span data-stu-id="4b986-110">String</span></span>     | <span data-ttu-id="4b986-111">件名の id。</span><span class="sxs-lookup"><span data-stu-id="4b986-111">The id of the subject.</span></span>|
|<span data-ttu-id="4b986-112">type</span><span class="sxs-lookup"><span data-stu-id="4b986-112">type</span></span>       |<span data-ttu-id="4b986-113">String</span><span class="sxs-lookup"><span data-stu-id="4b986-113">String</span></span>     |<span data-ttu-id="4b986-114">件名の種類。</span><span class="sxs-lookup"><span data-stu-id="4b986-114">The type of the subject.</span></span> <span data-ttu-id="4b986-115">この値は、 ``User``、 ``Group``、と``ServicePrincipal``することができます。</span><span class="sxs-lookup"><span data-stu-id="4b986-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="4b986-116">displayName</span><span class="sxs-lookup"><span data-stu-id="4b986-116">displayName</span></span>|<span data-ttu-id="4b986-117">文字列</span><span class="sxs-lookup"><span data-stu-id="4b986-117">String</span></span>     |<span data-ttu-id="4b986-118">件名の表示名。</span><span class="sxs-lookup"><span data-stu-id="4b986-118">The display name of the subject.</span></span>|
|<span data-ttu-id="4b986-119">email</span><span class="sxs-lookup"><span data-stu-id="4b986-119">email</span></span>      |<span data-ttu-id="4b986-120">String</span><span class="sxs-lookup"><span data-stu-id="4b986-120">String</span></span>     |<span data-ttu-id="4b986-121">ユーザーの件名の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="4b986-121">The email address of the user subject.</span></span> <span data-ttu-id="4b986-122">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="4b986-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="4b986-123">principalName</span><span class="sxs-lookup"><span data-stu-id="4b986-123">principalName</span></span>|<span data-ttu-id="4b986-124">String</span><span class="sxs-lookup"><span data-stu-id="4b986-124">String</span></span>   |<span data-ttu-id="4b986-125">ユーザーの件名のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="4b986-125">The principal name of the user subject.</span></span> <span data-ttu-id="4b986-126">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="4b986-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="4b986-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="4b986-127">Relationships</span></span>
<span data-ttu-id="4b986-128">なし</span><span class="sxs-lookup"><span data-stu-id="4b986-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="4b986-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4b986-129">JSON representation</span></span>

<span data-ttu-id="4b986-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4b986-130">Here is a JSON representation of the resource.</span></span>

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
  "suppressions": []
}
-->
