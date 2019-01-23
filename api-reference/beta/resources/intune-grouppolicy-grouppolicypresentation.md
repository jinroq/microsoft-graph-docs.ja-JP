---
title: groupPolicyPresentation リソースの種類
description: グループ ポリシーの定義の他のオプションのいずれかの表示のプレゼンテーションの基本エンティティです。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 736b599eaf310bc63530daa45ffa1aee7ede4c3f
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430543"
---
# <a name="grouppolicypresentation-resource-type"></a><span data-ttu-id="e09e9-103">groupPolicyPresentation リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e09e9-103">groupPolicyPresentation resource type</span></span>

> <span data-ttu-id="e09e9-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e09e9-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e09e9-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e09e9-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e09e9-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e09e9-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e09e9-107">グループ ポリシーの定義の他のオプションのいずれかの表示のプレゼンテーションの基本エンティティです。</span><span class="sxs-lookup"><span data-stu-id="e09e9-107">The base entity for the display presentation of any of the additional options in a group policy definition.</span></span>

## <a name="methods"></a><span data-ttu-id="e09e9-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e09e9-108">Methods</span></span>
|<span data-ttu-id="e09e9-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e09e9-109">Method</span></span>|<span data-ttu-id="e09e9-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e09e9-110">Return Type</span></span>|<span data-ttu-id="e09e9-111">説明</span><span class="sxs-lookup"><span data-stu-id="e09e9-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e09e9-112">GroupPolicyPresentation を取得します。</span><span class="sxs-lookup"><span data-stu-id="e09e9-112">Get groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-get.md)|[<span data-ttu-id="e09e9-113">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="e09e9-113">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="e09e9-114">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e09e9-114">Read properties and relationships of the [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|
|[<span data-ttu-id="e09e9-115">GroupPolicyPresentation を更新します。</span><span class="sxs-lookup"><span data-stu-id="e09e9-115">Update groupPolicyPresentation</span></span>](../api/intune-grouppolicy-grouppolicypresentation-update.md)|[<span data-ttu-id="e09e9-116">groupPolicyPresentation</span><span class="sxs-lookup"><span data-stu-id="e09e9-116">groupPolicyPresentation</span></span>](../resources/intune-grouppolicy-grouppolicypresentation.md)|<span data-ttu-id="e09e9-117">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e09e9-117">Update the properties of a [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e09e9-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e09e9-118">Properties</span></span>
|<span data-ttu-id="e09e9-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e09e9-119">Property</span></span>|<span data-ttu-id="e09e9-120">型</span><span class="sxs-lookup"><span data-stu-id="e09e9-120">Type</span></span>|<span data-ttu-id="e09e9-121">説明</span><span class="sxs-lookup"><span data-stu-id="e09e9-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e09e9-122">label</span><span class="sxs-lookup"><span data-stu-id="e09e9-122">label</span></span>|<span data-ttu-id="e09e9-123">String</span><span class="sxs-lookup"><span data-stu-id="e09e9-123">String</span></span>|<span data-ttu-id="e09e9-124">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="e09e9-124">Localized text label for any presentation entity.</span></span> <span data-ttu-id="e09e9-125">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="e09e9-125">The default value is empty.</span></span>|
|<span data-ttu-id="e09e9-126">id</span><span class="sxs-lookup"><span data-stu-id="e09e9-126">id</span></span>|<span data-ttu-id="e09e9-127">String</span><span class="sxs-lookup"><span data-stu-id="e09e9-127">String</span></span>|<span data-ttu-id="e09e9-128">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e09e9-128">Key of the entity.</span></span>|
|<span data-ttu-id="e09e9-129">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e09e9-129">lastModifiedDateTime</span></span>|<span data-ttu-id="e09e9-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e09e9-130">DateTimeOffset</span></span>|<span data-ttu-id="e09e9-131">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="e09e9-131">The date and time the entity was last modified.</span></span>|

## <a name="relationships"></a><span data-ttu-id="e09e9-132">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e09e9-132">Relationships</span></span>
|<span data-ttu-id="e09e9-133">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e09e9-133">Relationship</span></span>|<span data-ttu-id="e09e9-134">型</span><span class="sxs-lookup"><span data-stu-id="e09e9-134">Type</span></span>|<span data-ttu-id="e09e9-135">説明</span><span class="sxs-lookup"><span data-stu-id="e09e9-135">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e09e9-136">definition</span><span class="sxs-lookup"><span data-stu-id="e09e9-136">definition</span></span>|[<span data-ttu-id="e09e9-137">groupPolicyDefinition</span><span class="sxs-lookup"><span data-stu-id="e09e9-137">groupPolicyDefinition</span></span>](../resources/intune-grouppolicy-grouppolicydefinition.md)|<span data-ttu-id="e09e9-138">プレゼンテーションに関連付けられているグループ ポリシーの定義です。</span><span class="sxs-lookup"><span data-stu-id="e09e9-138">The group policy definition associated with the presentation.</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e09e9-139">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e09e9-139">JSON Representation</span></span>
<span data-ttu-id="e09e9-140">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e09e9-140">Here is a JSON representation of the resource.</span></span>
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




