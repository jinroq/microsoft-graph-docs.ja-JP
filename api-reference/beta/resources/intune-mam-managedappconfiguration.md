---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 67b445c5f7882bb4befc3e2c5cc46e26c5cf50fc
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29405675"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="e5e92-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e5e92-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="e5e92-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e5e92-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e5e92-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e5e92-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e5e92-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e5e92-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e5e92-107">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="e5e92-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="e5e92-108">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e5e92-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5e92-109">Methods</span></span>
|<span data-ttu-id="e5e92-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e5e92-110">Method</span></span>|<span data-ttu-id="e5e92-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e5e92-111">Return Type</span></span>|<span data-ttu-id="e5e92-112">説明</span><span class="sxs-lookup"><span data-stu-id="e5e92-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e5e92-113">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="e5e92-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="e5e92-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e92-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="e5e92-115">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e5e92-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e5e92-116">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="e5e92-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="e5e92-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e5e92-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="e5e92-118">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e5e92-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e5e92-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5e92-119">Properties</span></span>
|<span data-ttu-id="e5e92-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e5e92-120">Property</span></span>|<span data-ttu-id="e5e92-121">型</span><span class="sxs-lookup"><span data-stu-id="e5e92-121">Type</span></span>|<span data-ttu-id="e5e92-122">説明</span><span class="sxs-lookup"><span data-stu-id="e5e92-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e5e92-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e5e92-123">displayName</span></span>|<span data-ttu-id="e5e92-124">String</span><span class="sxs-lookup"><span data-stu-id="e5e92-124">String</span></span>|<span data-ttu-id="e5e92-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e5e92-125">Policy display name.</span></span> <span data-ttu-id="e5e92-126">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-127">説明</span><span class="sxs-lookup"><span data-stu-id="e5e92-127">description</span></span>|<span data-ttu-id="e5e92-128">String</span><span class="sxs-lookup"><span data-stu-id="e5e92-128">String</span></span>|<span data-ttu-id="e5e92-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e5e92-129">The policy's description.</span></span> <span data-ttu-id="e5e92-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e5e92-131">createdDateTime</span></span>|<span data-ttu-id="e5e92-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e92-132">DateTimeOffset</span></span>|<span data-ttu-id="e5e92-133">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e5e92-133">The date and time the policy was created.</span></span> <span data-ttu-id="e5e92-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e5e92-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e5e92-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e5e92-136">DateTimeOffset</span></span>|<span data-ttu-id="e5e92-137">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e5e92-137">Last time the policy was modified.</span></span> <span data-ttu-id="e5e92-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-139">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="e5e92-139">roleScopeTagIds</span></span>|<span data-ttu-id="e5e92-140">String コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e92-140">String collection</span></span>|<span data-ttu-id="e5e92-141">このエンティティ インスタンスのスコープのタグのリストです。</span><span class="sxs-lookup"><span data-stu-id="e5e92-141">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="e5e92-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-143">id</span><span class="sxs-lookup"><span data-stu-id="e5e92-143">id</span></span>|<span data-ttu-id="e5e92-144">String</span><span class="sxs-lookup"><span data-stu-id="e5e92-144">String</span></span>|<span data-ttu-id="e5e92-145">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e5e92-145">Key of the entity.</span></span> <span data-ttu-id="e5e92-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-147">version</span><span class="sxs-lookup"><span data-stu-id="e5e92-147">version</span></span>|<span data-ttu-id="e5e92-148">String</span><span class="sxs-lookup"><span data-stu-id="e5e92-148">String</span></span>|<span data-ttu-id="e5e92-149">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e5e92-149">Version of the entity.</span></span> <span data-ttu-id="e5e92-150">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e5e92-150">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e5e92-151">customSettings</span><span class="sxs-lookup"><span data-stu-id="e5e92-151">customSettings</span></span>|<span data-ttu-id="e5e92-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e5e92-152">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e5e92-153">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="e5e92-153">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="e5e92-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e5e92-154">Relationships</span></span>
<span data-ttu-id="e5e92-155">なし</span><span class="sxs-lookup"><span data-stu-id="e5e92-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="e5e92-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e5e92-156">JSON Representation</span></span>
<span data-ttu-id="e5e92-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e5e92-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.managedAppConfiguration"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.managedAppConfiguration",
  "displayName": "String",
  "description": "String",
  "createdDateTime": "String (timestamp)",
  "lastModifiedDateTime": "String (timestamp)",
  "roleScopeTagIds": [
    "String"
  ],
  "id": "String (identifier)",
  "version": "String",
  "customSettings": [
    {
      "@odata.type": "microsoft.graph.keyValuePair",
      "name": "String",
      "value": "String"
    }
  ]
}
```




