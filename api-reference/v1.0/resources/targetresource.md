---
title: targetResource リソースの種類
description: 監査アクティビティに関連付けられているターゲットリソースの種類を表します。
localization_priority: Normal
author: dhanyahk
ms.prod: azure-ad
ms.openlocfilehash: 33a381d6088245be235f37549184183443fe3237
ms.sourcegitcommit: b8d01acfc1cb7610a0e1f5c18065da415bae0777
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/06/2019
ms.locfileid: "33629216"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="ef4a3-103">targetResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="ef4a3-103">targetResource resource type</span></span>

<span data-ttu-id="ef4a3-104">監査アクティビティに関連付けられているターゲットリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-104">Represents target resource types associated with audit activity.</span></span> 

## <a name="properties"></a><span data-ttu-id="ef4a3-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef4a3-105">Properties</span></span>

| <span data-ttu-id="ef4a3-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ef4a3-106">Property</span></span>     | <span data-ttu-id="ef4a3-107">型</span><span class="sxs-lookup"><span data-stu-id="ef4a3-107">Type</span></span>   |<span data-ttu-id="ef4a3-108">説明</span><span class="sxs-lookup"><span data-stu-id="ef4a3-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="ef4a3-109">id</span><span class="sxs-lookup"><span data-stu-id="ef4a3-109">id</span></span>|<span data-ttu-id="ef4a3-110">文字列</span><span class="sxs-lookup"><span data-stu-id="ef4a3-110">String</span></span>|<span data-ttu-id="ef4a3-111">リソースの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="ef4a3-112">displayName</span><span class="sxs-lookup"><span data-stu-id="ef4a3-112">displayName</span></span>|<span data-ttu-id="ef4a3-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="ef4a3-113">String</span></span>|<span data-ttu-id="ef4a3-114">リソースに対して定義されている表示名を示します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="ef4a3-115">通常、リソースの作成時に指定されます。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="ef4a3-116">type</span><span class="sxs-lookup"><span data-stu-id="ef4a3-116">type</span></span>|<span data-ttu-id="ef4a3-117">String</span><span class="sxs-lookup"><span data-stu-id="ef4a3-117">String</span></span>|<span data-ttu-id="ef4a3-118">リソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-118">Describes the resource type.</span></span>  <span data-ttu-id="ef4a3-119">値の例`Application`に`Group`は`ServicePrincipal`、、 `User`、、などがあります。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="ef4a3-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ef4a3-120">userPrincipalName</span></span>|<span data-ttu-id="ef4a3-121">String</span><span class="sxs-lookup"><span data-stu-id="ef4a3-121">String</span></span>|<span data-ttu-id="ef4a3-122">**型**がに`User`設定されている場合、これにはアクションを開始したユーザー名が含まれます。`null`その他の種類の場合。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="ef4a3-123">groupType</span><span class="sxs-lookup"><span data-stu-id="ef4a3-123">groupType</span></span>|<span data-ttu-id="ef4a3-124">String</span><span class="sxs-lookup"><span data-stu-id="ef4a3-124">String</span></span>|<span data-ttu-id="ef4a3-125">**型**がに`Group`設定されている場合は、グループの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="ef4a3-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="ef4a3-126">modifiedProperties</span></span>|<span data-ttu-id="ef4a3-127">[modifiedProperty](modifiedproperty.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="ef4a3-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="ef4a3-128">変更された各属性の名前、古い値、新しい値を示します。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="ef4a3-129">プロパティの値は、操作の**種類**によって異なります。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="ef4a3-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="ef4a3-130">JSON representation</span></span>

<span data-ttu-id="ef4a3-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="ef4a3-131">Here is a JSON representation of the resource.</span></span>

<!-- {
  "blockType": "resource",
  "optionalProperties": [

  ],
  "@odata.type": "microsoft.graph.targetResource"
}-->

```json
{
  "id": "String",
  "displayName": "String",
  "type": "String",
  "userPrincipalName": "String",
  "groupType": "String",
  "modifiedProperties": [{"@odata.type": "microsoft.graph.modifiedProperty"}]
}
```


<!-- uuid: 8fcb5dbc-d5aa-4681-8e31-b001d5168d79
2015-10-25 14:57:30 UTC -->
<!-- {
  "type": "#page.annotation",
  "description": "targetResource resource",
  "keywords": "",
  "section": "documentation",
  "tocPath": ""
}-->
