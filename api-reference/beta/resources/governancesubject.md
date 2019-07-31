---
title: governanceSubject リソースの種類
description: 特権 Id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。
localization_priority: Normal
doc_type: resourcePageType
ms.prod: ''
author: ''
ms.openlocfilehash: 26f6c6904de97fc96eb1b29b9bcbc376bcf69c61
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36005976"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="f7020-103">governanceSubject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="f7020-103">governanceSubject resource type</span></span>

[!INCLUDE [beta-disclaimer](../../includes/beta-disclaimer.md)]

<span data-ttu-id="f7020-104">特権 Id 管理 (PIM) で管理されているユーザー、グループ、およびサービスプリンシパルを表します。</span><span class="sxs-lookup"><span data-stu-id="f7020-104">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="f7020-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7020-105">Properties</span></span>
| <span data-ttu-id="f7020-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f7020-106">Property</span></span>  | <span data-ttu-id="f7020-107">型</span><span class="sxs-lookup"><span data-stu-id="f7020-107">Type</span></span>       |<span data-ttu-id="f7020-108">説明</span><span class="sxs-lookup"><span data-stu-id="f7020-108">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="f7020-109">id</span><span class="sxs-lookup"><span data-stu-id="f7020-109">id</span></span>         |<span data-ttu-id="f7020-110">文字列</span><span class="sxs-lookup"><span data-stu-id="f7020-110">String</span></span>     | <span data-ttu-id="f7020-111">件名の id。</span><span class="sxs-lookup"><span data-stu-id="f7020-111">The id of the subject.</span></span>|
|<span data-ttu-id="f7020-112">type</span><span class="sxs-lookup"><span data-stu-id="f7020-112">type</span></span>       |<span data-ttu-id="f7020-113">String</span><span class="sxs-lookup"><span data-stu-id="f7020-113">String</span></span>     |<span data-ttu-id="f7020-114">件名の種類。</span><span class="sxs-lookup"><span data-stu-id="f7020-114">The type of the subject.</span></span> <span data-ttu-id="f7020-115">この値は、 ``User``、 ``Group``、と``ServicePrincipal``することができます。</span><span class="sxs-lookup"><span data-stu-id="f7020-115">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="f7020-116">displayName</span><span class="sxs-lookup"><span data-stu-id="f7020-116">displayName</span></span>|<span data-ttu-id="f7020-117">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="f7020-117">String</span></span>     |<span data-ttu-id="f7020-118">件名の表示名。</span><span class="sxs-lookup"><span data-stu-id="f7020-118">The display name of the subject.</span></span>|
|<span data-ttu-id="f7020-119">メール</span><span class="sxs-lookup"><span data-stu-id="f7020-119">email</span></span>      |<span data-ttu-id="f7020-120">String</span><span class="sxs-lookup"><span data-stu-id="f7020-120">String</span></span>     |<span data-ttu-id="f7020-121">ユーザーの件名の電子メールアドレス。</span><span class="sxs-lookup"><span data-stu-id="f7020-121">The email address of the user subject.</span></span> <span data-ttu-id="f7020-122">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="f7020-122">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="f7020-123">principalName</span><span class="sxs-lookup"><span data-stu-id="f7020-123">principalName</span></span>|<span data-ttu-id="f7020-124">String</span><span class="sxs-lookup"><span data-stu-id="f7020-124">String</span></span>   |<span data-ttu-id="f7020-125">ユーザーの件名のプリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="f7020-125">The principal name of the user subject.</span></span> <span data-ttu-id="f7020-126">件名が他の種類の場合は、空になります。</span><span class="sxs-lookup"><span data-stu-id="f7020-126">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="f7020-127">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="f7020-127">Relationships</span></span>
<span data-ttu-id="f7020-128">なし</span><span class="sxs-lookup"><span data-stu-id="f7020-128">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="f7020-129">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="f7020-129">JSON representation</span></span>

<span data-ttu-id="f7020-130">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="f7020-130">Here is a JSON representation of the resource.</span></span>

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
