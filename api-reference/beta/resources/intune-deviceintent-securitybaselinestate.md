---
title: securityBaselineState リソースの種類
description: デバイスのセキュリティベースラインの状態。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 3c81a3d351c7c1e854c26e05e32f8426ffdc0631
ms.sourcegitcommit: 0ce657622f42c510a104156a96bf1f1f040bc1cd
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/24/2019
ms.locfileid: "32562245"
---
# <a name="securitybaselinestate-resource-type"></a><span data-ttu-id="e62b4-103">securityBaselineState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e62b4-103">securityBaselineState resource type</span></span>

> <span data-ttu-id="e62b4-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e62b4-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e62b4-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e62b4-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e62b4-106">デバイスのセキュリティベースラインの状態。</span><span class="sxs-lookup"><span data-stu-id="e62b4-106">Security baseline state for a device.</span></span>

## <a name="methods"></a><span data-ttu-id="e62b4-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="e62b4-107">Methods</span></span>
|<span data-ttu-id="e62b4-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="e62b4-108">Method</span></span>|<span data-ttu-id="e62b4-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e62b4-109">Return Type</span></span>|<span data-ttu-id="e62b4-110">説明</span><span class="sxs-lookup"><span data-stu-id="e62b4-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e62b4-111">リスト securityBaselineStates</span><span class="sxs-lookup"><span data-stu-id="e62b4-111">List securityBaselineStates</span></span>](../api/intune-deviceintent-securitybaselinestate-list.md)|<span data-ttu-id="e62b4-112">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e62b4-112">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) collection</span></span>|<span data-ttu-id="e62b4-113">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e62b4-113">List properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) objects.</span></span>|
|[<span data-ttu-id="e62b4-114">securityBaselineState を取得する</span><span class="sxs-lookup"><span data-stu-id="e62b4-114">Get securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-get.md)|[<span data-ttu-id="e62b4-115">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e62b4-115">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e62b4-116">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e62b4-116">Read properties and relationships of the [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|
|[<span data-ttu-id="e62b4-117">securityBaselineState を作成する</span><span class="sxs-lookup"><span data-stu-id="e62b4-117">Create securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-create.md)|[<span data-ttu-id="e62b4-118">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e62b4-118">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e62b4-119">新しい[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="e62b4-119">Create a new [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|
|[<span data-ttu-id="e62b4-120">securityBaselineState の削除</span><span class="sxs-lookup"><span data-stu-id="e62b4-120">Delete securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-delete.md)|<span data-ttu-id="e62b4-121">なし</span><span class="sxs-lookup"><span data-stu-id="e62b4-121">None</span></span>|<span data-ttu-id="e62b4-122">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="e62b4-122">Deletes a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md).</span></span>|
|[<span data-ttu-id="e62b4-123">securityBaselineState の更新</span><span class="sxs-lookup"><span data-stu-id="e62b4-123">Update securityBaselineState</span></span>](../api/intune-deviceintent-securitybaselinestate-update.md)|[<span data-ttu-id="e62b4-124">securityBaselineState</span><span class="sxs-lookup"><span data-stu-id="e62b4-124">securityBaselineState</span></span>](../resources/intune-deviceintent-securitybaselinestate.md)|<span data-ttu-id="e62b4-125">[securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e62b4-125">Update the properties of a [securityBaselineState](../resources/intune-deviceintent-securitybaselinestate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e62b4-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e62b4-126">Properties</span></span>
|<span data-ttu-id="e62b4-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e62b4-127">Property</span></span>|<span data-ttu-id="e62b4-128">型</span><span class="sxs-lookup"><span data-stu-id="e62b4-128">Type</span></span>|<span data-ttu-id="e62b4-129">説明</span><span class="sxs-lookup"><span data-stu-id="e62b4-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62b4-130">id</span><span class="sxs-lookup"><span data-stu-id="e62b4-130">id</span></span>|<span data-ttu-id="e62b4-131">String</span><span class="sxs-lookup"><span data-stu-id="e62b4-131">String</span></span>|<span data-ttu-id="e62b4-132">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e62b4-132">Key of the entity.</span></span>|
|<span data-ttu-id="e62b4-133">securityBaselineTemplateId</span><span class="sxs-lookup"><span data-stu-id="e62b4-133">securityBaselineTemplateId</span></span>|<span data-ttu-id="e62b4-134">String</span><span class="sxs-lookup"><span data-stu-id="e62b4-134">String</span></span>|<span data-ttu-id="e62b4-135">セキュリティ基準テンプレート id</span><span class="sxs-lookup"><span data-stu-id="e62b4-135">The security baseline template id</span></span>|
|<span data-ttu-id="e62b4-136">displayName</span><span class="sxs-lookup"><span data-stu-id="e62b4-136">displayName</span></span>|<span data-ttu-id="e62b4-137">String</span><span class="sxs-lookup"><span data-stu-id="e62b4-137">String</span></span>|<span data-ttu-id="e62b4-138">セキュリティベースラインの表示名</span><span class="sxs-lookup"><span data-stu-id="e62b4-138">The display name of the security baseline</span></span>|

## <a name="relationships"></a><span data-ttu-id="e62b4-139">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e62b4-139">Relationships</span></span>
|<span data-ttu-id="e62b4-140">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e62b4-140">Relationship</span></span>|<span data-ttu-id="e62b4-141">型</span><span class="sxs-lookup"><span data-stu-id="e62b4-141">Type</span></span>|<span data-ttu-id="e62b4-142">説明</span><span class="sxs-lookup"><span data-stu-id="e62b4-142">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e62b4-143">settingStates</span><span class="sxs-lookup"><span data-stu-id="e62b4-143">settingStates</span></span>|<span data-ttu-id="e62b4-144">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="e62b4-144">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="e62b4-145">デバイスのさまざまな設定のセキュリティベースライン状態</span><span class="sxs-lookup"><span data-stu-id="e62b4-145">The security baseline state for different settings for a device</span></span>|

## <a name="json-representation"></a><span data-ttu-id="e62b4-146">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e62b4-146">JSON Representation</span></span>
<span data-ttu-id="e62b4-147">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e62b4-147">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineState",
  "id": "String (identifier)",
  "securityBaselineTemplateId": "String",
  "displayName": "String"
}
```



