---
title: securityBaselineSettingState リソースの種類
description: デバイスの設定のセキュリティベースラインコンプライアンスの状態
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: ab5dd14c0929c58b9c076d1115d487e560d80333
ms.sourcegitcommit: 77f485ec03a8c917f59d2fbed4df1ec755f3da58
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 04/08/2019
ms.locfileid: "31522581"
---
# <a name="securitybaselinesettingstate-resource-type"></a><span data-ttu-id="68f36-103">securityBaselineSettingState リソースの種類</span><span class="sxs-lookup"><span data-stu-id="68f36-103">securityBaselineSettingState resource type</span></span>

> <span data-ttu-id="68f36-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="68f36-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="68f36-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="68f36-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="68f36-106">デバイスの設定のセキュリティベースラインコンプライアンスの状態</span><span class="sxs-lookup"><span data-stu-id="68f36-106">The security baseline compliance state of a setting for a device</span></span>

## <a name="methods"></a><span data-ttu-id="68f36-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="68f36-107">Methods</span></span>
|<span data-ttu-id="68f36-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="68f36-108">Method</span></span>|<span data-ttu-id="68f36-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="68f36-109">Return Type</span></span>|<span data-ttu-id="68f36-110">説明</span><span class="sxs-lookup"><span data-stu-id="68f36-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="68f36-111">リスト securityBaselineSettingStates</span><span class="sxs-lookup"><span data-stu-id="68f36-111">List securityBaselineSettingStates</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-list.md)|<span data-ttu-id="68f36-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="68f36-112">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) collection</span></span>|<span data-ttu-id="68f36-113">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="68f36-113">List properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) objects.</span></span>|
|[<span data-ttu-id="68f36-114">securityBaselineSettingState を取得する</span><span class="sxs-lookup"><span data-stu-id="68f36-114">Get securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-get.md)|[<span data-ttu-id="68f36-115">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="68f36-115">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="68f36-116">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="68f36-116">Read properties and relationships of the [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="68f36-117">securityBaselineSettingState を作成する</span><span class="sxs-lookup"><span data-stu-id="68f36-117">Create securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-create.md)|[<span data-ttu-id="68f36-118">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="68f36-118">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="68f36-119">新しい[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="68f36-119">Create a new [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|
|[<span data-ttu-id="68f36-120">securityBaselineSettingState の削除</span><span class="sxs-lookup"><span data-stu-id="68f36-120">Delete securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-delete.md)|<span data-ttu-id="68f36-121">なし</span><span class="sxs-lookup"><span data-stu-id="68f36-121">None</span></span>|<span data-ttu-id="68f36-122">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="68f36-122">Deletes a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md).</span></span>|
|[<span data-ttu-id="68f36-123">securityBaselineSettingState の更新</span><span class="sxs-lookup"><span data-stu-id="68f36-123">Update securityBaselineSettingState</span></span>](../api/intune-deviceintent-securitybaselinesettingstate-update.md)|[<span data-ttu-id="68f36-124">securityBaselineSettingState</span><span class="sxs-lookup"><span data-stu-id="68f36-124">securityBaselineSettingState</span></span>](../resources/intune-deviceintent-securitybaselinesettingstate.md)|<span data-ttu-id="68f36-125">[securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="68f36-125">Update the properties of a [securityBaselineSettingState](../resources/intune-deviceintent-securitybaselinesettingstate.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="68f36-126">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68f36-126">Properties</span></span>
|<span data-ttu-id="68f36-127">プロパティ</span><span class="sxs-lookup"><span data-stu-id="68f36-127">Property</span></span>|<span data-ttu-id="68f36-128">型</span><span class="sxs-lookup"><span data-stu-id="68f36-128">Type</span></span>|<span data-ttu-id="68f36-129">説明</span><span class="sxs-lookup"><span data-stu-id="68f36-129">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="68f36-130">id</span><span class="sxs-lookup"><span data-stu-id="68f36-130">id</span></span>|<span data-ttu-id="68f36-131">String</span><span class="sxs-lookup"><span data-stu-id="68f36-131">String</span></span>|<span data-ttu-id="68f36-132">エンティティの一意識別子</span><span class="sxs-lookup"><span data-stu-id="68f36-132">Unique identifier of the entity</span></span>|
|<span data-ttu-id="68f36-133">settingName</span><span class="sxs-lookup"><span data-stu-id="68f36-133">settingName</span></span>|<span data-ttu-id="68f36-134">String</span><span class="sxs-lookup"><span data-stu-id="68f36-134">String</span></span>|<span data-ttu-id="68f36-135">レポートされている設定の名前</span><span class="sxs-lookup"><span data-stu-id="68f36-135">The setting name that is being reported</span></span>|
|<span data-ttu-id="68f36-136">state</span><span class="sxs-lookup"><span data-stu-id="68f36-136">state</span></span>|[<span data-ttu-id="68f36-137">securityBaselineComplianceState</span><span class="sxs-lookup"><span data-stu-id="68f36-137">securityBaselineComplianceState</span></span>](../resources/intune-deviceintent-securitybaselinecompliancestate.md)|<span data-ttu-id="68f36-138">セキュリティベースライン設定のコンプライアンス状態。</span><span class="sxs-lookup"><span data-stu-id="68f36-138">The compliance state of the security baseline setting.</span></span> <span data-ttu-id="68f36-139">可能な値は `unknown`、`secure`、`notApplicable`、`notSecure`、`error`、`conflict` です。</span><span class="sxs-lookup"><span data-stu-id="68f36-139">Possible values are: `unknown`, `secure`, `notApplicable`, `notSecure`, `error`, `conflict`.</span></span>|
|<span data-ttu-id="68f36-140">settingcategoryid</span><span class="sxs-lookup"><span data-stu-id="68f36-140">settingCategoryId</span></span>|<span data-ttu-id="68f36-141">文字列</span><span class="sxs-lookup"><span data-stu-id="68f36-141">String</span></span>|<span data-ttu-id="68f36-142">この設定が属する設定カテゴリ id</span><span class="sxs-lookup"><span data-stu-id="68f36-142">The setting category id which this setting belongs to</span></span>|

## <a name="relationships"></a><span data-ttu-id="68f36-143">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="68f36-143">Relationships</span></span>
<span data-ttu-id="68f36-144">なし</span><span class="sxs-lookup"><span data-stu-id="68f36-144">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="68f36-145">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="68f36-145">JSON Representation</span></span>
<span data-ttu-id="68f36-146">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="68f36-146">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.securityBaselineSettingState"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.securityBaselineSettingState",
  "id": "String (identifier)",
  "settingName": "String",
  "state": "String",
  "settingCategoryId": "String"
}
```



