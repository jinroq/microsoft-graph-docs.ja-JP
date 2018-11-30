---
title: governanceSubject リソースの種類
description: ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。
ms.openlocfilehash: c2129a0da488d4e7f425d6ef3596a955269e0da8
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27067103"
---
# <a name="governancesubject-resource-type"></a><span data-ttu-id="a0be3-103">governanceSubject リソースの種類</span><span class="sxs-lookup"><span data-stu-id="a0be3-103">governanceSubject resource type</span></span>

> <span data-ttu-id="a0be3-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a0be3-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="a0be3-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a0be3-105">Use of these APIs in production applications is not supported.</span></span>

<span data-ttu-id="a0be3-106">ユーザー、グループ、および権限を持つユーザー情報管理 (PIM) では管理されているサービス ・ プリンシパルを表します。</span><span class="sxs-lookup"><span data-stu-id="a0be3-106">Represents users, groups, and service principals being managed in Privileged Identity Management (PIM).</span></span>


## <a name="properties"></a><span data-ttu-id="a0be3-107">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0be3-107">Properties</span></span>
| <span data-ttu-id="a0be3-108">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a0be3-108">Property</span></span>  | <span data-ttu-id="a0be3-109">型</span><span class="sxs-lookup"><span data-stu-id="a0be3-109">Type</span></span>       |<span data-ttu-id="a0be3-110">説明</span><span class="sxs-lookup"><span data-stu-id="a0be3-110">Description</span></span>|
|:----------|:----------|:----------|
|<span data-ttu-id="a0be3-111">id</span><span class="sxs-lookup"><span data-stu-id="a0be3-111">id</span></span>         |<span data-ttu-id="a0be3-112">String</span><span class="sxs-lookup"><span data-stu-id="a0be3-112">String</span></span>     | <span data-ttu-id="a0be3-113">サブジェクトの id です。</span><span class="sxs-lookup"><span data-stu-id="a0be3-113">The id of the subject.</span></span>|
|<span data-ttu-id="a0be3-114">type</span><span class="sxs-lookup"><span data-stu-id="a0be3-114">type</span></span>       |<span data-ttu-id="a0be3-115">String</span><span class="sxs-lookup"><span data-stu-id="a0be3-115">String</span></span>     |<span data-ttu-id="a0be3-116">サブジェクトの種類。</span><span class="sxs-lookup"><span data-stu-id="a0be3-116">The type of the subject.</span></span> <span data-ttu-id="a0be3-117">値は、 ``User``、``Group``と``ServicePrincipal``。</span><span class="sxs-lookup"><span data-stu-id="a0be3-117">The value can be ``User``, ``Group``, and ``ServicePrincipal``.</span></span>|
|<span data-ttu-id="a0be3-118">displayName</span><span class="sxs-lookup"><span data-stu-id="a0be3-118">displayName</span></span>|<span data-ttu-id="a0be3-119">String</span><span class="sxs-lookup"><span data-stu-id="a0be3-119">String</span></span>     |<span data-ttu-id="a0be3-120">件名の表示名です。</span><span class="sxs-lookup"><span data-stu-id="a0be3-120">The display name of the subject.</span></span>|
|<span data-ttu-id="a0be3-121">email</span><span class="sxs-lookup"><span data-stu-id="a0be3-121">email</span></span>      |<span data-ttu-id="a0be3-122">String</span><span class="sxs-lookup"><span data-stu-id="a0be3-122">String</span></span>     |<span data-ttu-id="a0be3-123">ユーザーのサブジェクトの電子メール アドレスです。</span><span class="sxs-lookup"><span data-stu-id="a0be3-123">The email address of the user subject.</span></span> <span data-ttu-id="a0be3-124">件名は、他の種類では、空であるか。</span><span class="sxs-lookup"><span data-stu-id="a0be3-124">If the subject is in other types, it is empty.</span></span>|
|<span data-ttu-id="a0be3-125">principalName</span><span class="sxs-lookup"><span data-stu-id="a0be3-125">principalName</span></span>|<span data-ttu-id="a0be3-126">String</span><span class="sxs-lookup"><span data-stu-id="a0be3-126">String</span></span>   |<span data-ttu-id="a0be3-127">ユーザーのサブジェクトのプリンシパルの名前です。</span><span class="sxs-lookup"><span data-stu-id="a0be3-127">The principal name of the user subject.</span></span> <span data-ttu-id="a0be3-128">件名は、他の種類では、空であるか。</span><span class="sxs-lookup"><span data-stu-id="a0be3-128">If the subject is in other types, it is empty.</span></span>|

## <a name="relationships"></a><span data-ttu-id="a0be3-129">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="a0be3-129">Relationships</span></span>
<span data-ttu-id="a0be3-130">なし</span><span class="sxs-lookup"><span data-stu-id="a0be3-130">None</span></span>


## <a name="json-representation"></a><span data-ttu-id="a0be3-131">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="a0be3-131">JSON representation</span></span>

<span data-ttu-id="a0be3-132">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="a0be3-132">Here is a JSON representation of the resource.</span></span>

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
<!-- {
  "type": "#page.annotation",
  "description": "governanceSubject",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->