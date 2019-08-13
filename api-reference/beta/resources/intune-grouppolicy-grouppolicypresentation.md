---
title: groupPolicyPresentation リソースの種類
description: グループポリシー定義の追加オプションを表示するための基本エンティティ。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: ee950b7e4e292b9fb177778ff4df2dcb51641e54
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36331435"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="94481-103">groupPolicyPresentation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="94481-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="94481-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="94481-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="94481-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="94481-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="94481-106">グループポリシー定義の追加オプションを表示するための基本エンティティ。</span><span class="sxs-lookup"><span data-stu-id="94481-106">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="94481-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="94481-107">Methods</span></span>
|<span data-ttu-id="94481-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="94481-108">Method</span></span>|<span data-ttu-id="94481-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="94481-109">Return Type</span></span>|<span data-ttu-id="94481-110">説明</span><span class="sxs-lookup"><span data-stu-id="94481-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="94481-111">GroupPolicyPresentation を取得する</span><span class="sxs-lookup"><span data-stu-id="94481-111">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="94481-112">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="94481-112">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="94481-113">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="94481-113">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="94481-114">GroupPolicyPresentation の更新</span><span class="sxs-lookup"><span data-stu-id="94481-114">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="94481-115">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="94481-115">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="94481-116">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="94481-116">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="94481-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94481-117">Properties</span></span>
|<span data-ttu-id="94481-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="94481-118">Property</span></span>|<span data-ttu-id="94481-119">型</span><span class="sxs-lookup"><span data-stu-id="94481-119">Type</span></span>|<span data-ttu-id="94481-120">説明</span><span class="sxs-lookup"><span data-stu-id="94481-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94481-121">label</span><span class="sxs-lookup"><span data-stu-id="94481-121">label</span></span>|<span data-ttu-id="94481-122">String</span><span class="sxs-lookup"><span data-stu-id="94481-122">String</span></span>|<span data-ttu-id="94481-123">任意のプレゼンテーションエンティティのローカライズされたテキストラベル。</span><span class="sxs-lookup"><span data-stu-id="94481-123">Localized text label for any presentation entity.</span></span> <span data-ttu-id="94481-124">既定値は空白です。</span><span class="sxs-lookup"><span data-stu-id="94481-124">The default value is empty.</span></span>|
|<span data-ttu-id="94481-125">id</span><span class="sxs-lookup"><span data-stu-id="94481-125">id</span></span>|<span data-ttu-id="94481-126">String</span><span class="sxs-lookup"><span data-stu-id="94481-126">String</span></span>|<span data-ttu-id="94481-127">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="94481-127">Key of the entity.</span></span>|
|<span data-ttu-id="94481-128">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="94481-128">lastModifiedDateTime</span></span>|<span data-ttu-id="94481-129">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="94481-129">DateTimeOffset</span></span>|<span data-ttu-id="94481-130">エンティティが最後に変更された日付と時刻。</span><span class="sxs-lookup"><span data-stu-id="94481-130">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="94481-131">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94481-131">Relationships</span></span>
|<span data-ttu-id="94481-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="94481-132">Relationship</span></span>|<span data-ttu-id="94481-133">型</span><span class="sxs-lookup"><span data-stu-id="94481-133">Type</span></span>|<span data-ttu-id="94481-134">説明</span><span class="sxs-lookup"><span data-stu-id="94481-134">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="94481-135">definition</span><span class="sxs-lookup"><span data-stu-id="94481-135">definition</span></span>|[<span data-ttu-id="94481-136">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="94481-136">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="94481-137">プレゼンテーションに関連付けられたグループポリシーの定義。</span><span class="sxs-lookup"><span data-stu-id="94481-137">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="94481-138">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="94481-138">JSON Representation</span></span>
<span data-ttu-id="94481-139">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="94481-139">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.groupPolicyPresentation"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.groupPolicyPresentation",
  "label": "String",
  "id": "String (identifier)",
  "lastModifiedDateTime": "String (timestamp)"
}
```



