---
title: deviceCategory リソースの種類
description: これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。 レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: a0bb1e994bcf42ba91a55fdfc75946204d1f9b06
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32585337"
---
# <a name="devicecategory-resource-type"></a><span data-ttu-id="3f616-104">deviceCategory リソースの種類</span><span class="sxs-lookup"><span data-stu-id="3f616-104">deviceCategory resource type</span></span>

> <span data-ttu-id="3f616-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="3f616-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="3f616-106">デバイス カテゴリは、デバイスを整理する方法を提供します。</span><span class="sxs-lookup"><span data-stu-id="3f616-106">Device categories provides a way to organize your devices.</span></span> <span data-ttu-id="3f616-107">デバイス カテゴリを使用して、会社の管理者は、自社にとって意味のある、独自のカテゴリを定義できます。</span><span class="sxs-lookup"><span data-stu-id="3f616-107">Using device categories, company administrators can define their own categories that make sense to their company.</span></span><span data-ttu-id="3f616-108">これらのカテゴリは、Intune Azure コンソールでデバイスに適用することも、デバイスの登録時にユーザーが選択することもできます。</span><span class="sxs-lookup"><span data-stu-id="3f616-108"> These categories can then be applied to a device in the Intune Azure console or selected by a user during device enrollment.</span></span> <span data-ttu-id="3f616-109">レポートをフィルター処理し、デバイス カテゴリに基づく動的な Azure Active Directory デバイス グループを作成できます。</span><span class="sxs-lookup"><span data-stu-id="3f616-109">You can filter reports and create dynamic Azure Active Directory device groups based on device categories.</span></span>

## <a name="methods"></a><span data-ttu-id="3f616-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f616-110">Methods</span></span>
|<span data-ttu-id="3f616-111">メソッド</span><span class="sxs-lookup"><span data-stu-id="3f616-111">Method</span></span>|<span data-ttu-id="3f616-112">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="3f616-112">Return Type</span></span>|<span data-ttu-id="3f616-113">説明</span><span class="sxs-lookup"><span data-stu-id="3f616-113">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f616-114">[deviceCategories コレクションを一覧表示](../api/intune-shared-devicecategory-list.md)する</span><span class="sxs-lookup"><span data-stu-id="3f616-114">[List deviceCategories](../api/intune-shared-devicecategory-list.md) collection</span></span>|<span data-ttu-id="3f616-115">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="3f616-115">List properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) objects.</span></span>|
|[<span data-ttu-id="3f616-116">deviceCategory の取得</span><span class="sxs-lookup"><span data-stu-id="3f616-116">Get deviceCategory</span></span>](../api/intune-shared-devicecategory-get.md)|<span data-ttu-id="3f616-117">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティと関係を読み取ります。</span><span class="sxs-lookup"><span data-stu-id="3f616-117">Read properties and relationships of the [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|[<span data-ttu-id="3f616-118">deviceCategory の作成</span><span class="sxs-lookup"><span data-stu-id="3f616-118">Create deviceCategory</span></span>](../api/intune-shared-devicecategory-create.md)|<span data-ttu-id="3f616-119">新しい [deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="3f616-119">Create a new [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|
|<span data-ttu-id="3f616-120">[deviceCategory を削除](../api/intune-shared-devicecategory-delete.md)します。</span><span class="sxs-lookup"><span data-stu-id="3f616-120">[Delete deviceCategory](../api/intune-shared-devicecategory-delete.md).</span></span>|
|[<span data-ttu-id="3f616-121">deviceCategory の更新</span><span class="sxs-lookup"><span data-stu-id="3f616-121">Update deviceCategory</span></span>](../api/intune-shared-devicecategory-update.md)|<span data-ttu-id="3f616-122">[deviceCategory](../resources/intune-shared-devicecategory.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3f616-122">Update the properties of a [deviceCategory](../resources/intune-shared-devicecategory.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="3f616-123">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f616-123">Properties</span></span>
|<span data-ttu-id="3f616-124">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3f616-124">Property</span></span>|<span data-ttu-id="3f616-125">型</span><span class="sxs-lookup"><span data-stu-id="3f616-125">Type</span></span>|<span data-ttu-id="3f616-126">説明</span><span class="sxs-lookup"><span data-stu-id="3f616-126">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3f616-127">id</span><span class="sxs-lookup"><span data-stu-id="3f616-127">id</span></span>|<span data-ttu-id="3f616-128">文字列</span><span class="sxs-lookup"><span data-stu-id="3f616-128">String</span></span>|<span data-ttu-id="3f616-129">デバイス カテゴリの一意識別子。</span><span class="sxs-lookup"><span data-stu-id="3f616-129">Unique identifier for the device category.</span></span> <span data-ttu-id="3f616-130">読み取り専用です。</span><span class="sxs-lookup"><span data-stu-id="3f616-130">Read-only.</span></span>|
|<span data-ttu-id="3f616-131">**オンボーディング**</span><span class="sxs-lookup"><span data-stu-id="3f616-131">**Onboarding**</span></span>|
|<span data-ttu-id="3f616-132">displayName</span><span class="sxs-lookup"><span data-stu-id="3f616-132">displayName</span></span>|<span data-ttu-id="3f616-133">String</span><span class="sxs-lookup"><span data-stu-id="3f616-133">String</span></span>|<span data-ttu-id="3f616-134">デバイス カテゴリの表示名。</span><span class="sxs-lookup"><span data-stu-id="3f616-134">Display name for the device category.</span></span>|
|<span data-ttu-id="3f616-135">説明</span><span class="sxs-lookup"><span data-stu-id="3f616-135">description</span></span>|<span data-ttu-id="3f616-136">String</span><span class="sxs-lookup"><span data-stu-id="3f616-136">String</span></span>|<span data-ttu-id="3f616-137">デバイス カテゴリに関するオプションの説明。</span><span class="sxs-lookup"><span data-stu-id="3f616-137">Optional description for the device category.</span></span>|

## <a name="relationships"></a><span data-ttu-id="3f616-138">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="3f616-138">Relationships</span></span>
<span data-ttu-id="3f616-139">なし</span><span class="sxs-lookup"><span data-stu-id="3f616-139">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="3f616-140">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="3f616-140">JSON Representation</span></span>
<span data-ttu-id="3f616-141">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="3f616-141">Here is a JSON representation of the resource.</span></span>
<!--{
  "blockType": "resource",
  "keyProperty": "id",
  "baseType": "microsoft.graph.entity",
  "@odata.type": "microsoft.graph.deviceCategory"
}-->
``` json
{
  "@odata.type": "#microsoft.graph.deviceCategory",
  "id": "String (identifier)",
  "displayName": "String",
  "description": "String"
}
```



