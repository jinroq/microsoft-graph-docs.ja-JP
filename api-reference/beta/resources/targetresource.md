---
title: targetResource resource 複合型-Microsoft Graph API
description: 監査ログ報告組織 (テナント) アクティビティをサポートする Microsoft Graph API の targetResource entity resource 複合型を定義します。
author: davidmu1
localization_priority: Normal
ms.prod: azure-ad
ms.openlocfilehash: 0a52a8586d8bce211729b8dffe2a43129b94b30d
ms.sourcegitcommit: 33f1cf5b3b79bfba6a06b52d34e558a6ba327d21
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/31/2019
ms.locfileid: "34657652"
---
# <a name="targetresource-resource-type"></a><span data-ttu-id="4efc8-103">targetResource リソースの種類</span><span class="sxs-lookup"><span data-stu-id="4efc8-103">targetResource resource type</span></span>

<span data-ttu-id="4efc8-104">監査アクティビティに関連付けられているターゲットリソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-104">Represents target resource types associated with audit activity.</span></span> 


## <a name="properties"></a><span data-ttu-id="4efc8-105">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4efc8-105">Properties</span></span>

| <span data-ttu-id="4efc8-106">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4efc8-106">Property</span></span>     | <span data-ttu-id="4efc8-107">型</span><span class="sxs-lookup"><span data-stu-id="4efc8-107">Type</span></span>   |<span data-ttu-id="4efc8-108">説明</span><span class="sxs-lookup"><span data-stu-id="4efc8-108">Description</span></span>|
|:---------------|:--------|:----------|
|<span data-ttu-id="4efc8-109">id</span><span class="sxs-lookup"><span data-stu-id="4efc8-109">id</span></span>|<span data-ttu-id="4efc8-110">文字列</span><span class="sxs-lookup"><span data-stu-id="4efc8-110">String</span></span>|<span data-ttu-id="4efc8-111">リソースの一意の ID を示します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-111">Indicates the unique ID of the resource.</span></span>|
|<span data-ttu-id="4efc8-112">displayName</span><span class="sxs-lookup"><span data-stu-id="4efc8-112">displayName</span></span>|<span data-ttu-id="4efc8-113">文字列型 (String)</span><span class="sxs-lookup"><span data-stu-id="4efc8-113">String</span></span>|<span data-ttu-id="4efc8-114">リソースに対して定義されている表示名を示します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-114">Indicates the visible name defined for the resource.</span></span> <span data-ttu-id="4efc8-115">通常、リソースの作成時に指定されます。</span><span class="sxs-lookup"><span data-stu-id="4efc8-115">Typically specified when the resource is created.</span></span>|
|<span data-ttu-id="4efc8-116">type</span><span class="sxs-lookup"><span data-stu-id="4efc8-116">type</span></span>|<span data-ttu-id="4efc8-117">String</span><span class="sxs-lookup"><span data-stu-id="4efc8-117">String</span></span>|<span data-ttu-id="4efc8-118">リソースの種類を表します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-118">Describes the resource type.</span></span>  <span data-ttu-id="4efc8-119">値の例`Application`に`Group`は`ServicePrincipal`、、 `User`、、などがあります。</span><span class="sxs-lookup"><span data-stu-id="4efc8-119">Example values include `Application`, `Group`, `ServicePrincipal`, and `User`.</span></span>|
|<span data-ttu-id="4efc8-120">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="4efc8-120">userPrincipalName</span></span>|<span data-ttu-id="4efc8-121">String</span><span class="sxs-lookup"><span data-stu-id="4efc8-121">String</span></span>|<span data-ttu-id="4efc8-122">**型**がに`User`設定されている場合、これにはアクションを開始したユーザー名が含まれます。`null`その他の種類の場合。</span><span class="sxs-lookup"><span data-stu-id="4efc8-122">When **type** is set to `User`, this includes the user name that initiated the action; `null` for other types.</span></span>|
|<span data-ttu-id="4efc8-123">groupType</span><span class="sxs-lookup"><span data-stu-id="4efc8-123">groupType</span></span>|<span data-ttu-id="4efc8-124">String</span><span class="sxs-lookup"><span data-stu-id="4efc8-124">String</span></span>|<span data-ttu-id="4efc8-125">**型**がに`Group`設定されている場合は、グループの種類を示します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-125">When **type** is set to `Group`, this indicates the group type.</span></span>|
|<span data-ttu-id="4efc8-126">modifiedProperties</span><span class="sxs-lookup"><span data-stu-id="4efc8-126">modifiedProperties</span></span>|<span data-ttu-id="4efc8-127">[modifiedProperty](modifiedproperty.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="4efc8-127">[modifiedProperty](modifiedproperty.md) collection</span></span>|<span data-ttu-id="4efc8-128">変更された各属性の名前、古い値、新しい値を示します。</span><span class="sxs-lookup"><span data-stu-id="4efc8-128">Indicates name, old value and new value of each attribute that changed.</span></span> <span data-ttu-id="4efc8-129">プロパティの値は、操作の**種類**によって異なります。</span><span class="sxs-lookup"><span data-stu-id="4efc8-129">Property values depend on the operation **type**.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="4efc8-130">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="4efc8-130">JSON representation</span></span>

<span data-ttu-id="4efc8-131">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="4efc8-131">Here is a JSON representation of the resource.</span></span>

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
