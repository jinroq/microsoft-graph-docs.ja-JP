---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: f3c8db1f356890dc478833e7b77267a218f08bbc
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30148085"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="b0758-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="b0758-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="b0758-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="b0758-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="b0758-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="b0758-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="b0758-106">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="b0758-106">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="b0758-107">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-107">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="b0758-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0758-108">Methods</span></span>
|<span data-ttu-id="b0758-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="b0758-109">Method</span></span>|<span data-ttu-id="b0758-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="b0758-110">Return Type</span></span>|<span data-ttu-id="b0758-111">説明</span><span class="sxs-lookup"><span data-stu-id="b0758-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="b0758-112">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="b0758-112">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="b0758-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0758-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="b0758-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="b0758-114">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="b0758-115">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="b0758-115">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="b0758-116">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="b0758-116">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="b0758-117">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="b0758-117">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="b0758-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0758-118">Properties</span></span>
|<span data-ttu-id="b0758-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="b0758-119">Property</span></span>|<span data-ttu-id="b0758-120">型</span><span class="sxs-lookup"><span data-stu-id="b0758-120">Type</span></span>|<span data-ttu-id="b0758-121">説明</span><span class="sxs-lookup"><span data-stu-id="b0758-121">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="b0758-122">displayName</span><span class="sxs-lookup"><span data-stu-id="b0758-122">displayName</span></span>|<span data-ttu-id="b0758-123">String</span><span class="sxs-lookup"><span data-stu-id="b0758-123">String</span></span>|<span data-ttu-id="b0758-124">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="b0758-124">Policy display name.</span></span> <span data-ttu-id="b0758-125">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-125">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-126">説明</span><span class="sxs-lookup"><span data-stu-id="b0758-126">description</span></span>|<span data-ttu-id="b0758-127">String</span><span class="sxs-lookup"><span data-stu-id="b0758-127">String</span></span>|<span data-ttu-id="b0758-128">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="b0758-128">The policy's description.</span></span> <span data-ttu-id="b0758-129">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-129">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-130">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="b0758-130">createdDateTime</span></span>|<span data-ttu-id="b0758-131">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0758-131">DateTimeOffset</span></span>|<span data-ttu-id="b0758-132">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="b0758-132">The date and time the policy was created.</span></span> <span data-ttu-id="b0758-133">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-133">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-134">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="b0758-134">lastModifiedDateTime</span></span>|<span data-ttu-id="b0758-135">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="b0758-135">DateTimeOffset</span></span>|<span data-ttu-id="b0758-136">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="b0758-136">Last time the policy was modified.</span></span> <span data-ttu-id="b0758-137">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-137">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-138">roleScopeTagIds</span><span class="sxs-lookup"><span data-stu-id="b0758-138">roleScopeTagIds</span></span>|<span data-ttu-id="b0758-139">String collection</span><span class="sxs-lookup"><span data-stu-id="b0758-139">String collection</span></span>|<span data-ttu-id="b0758-140">このエンティティインスタンスの範囲タグのリスト。</span><span class="sxs-lookup"><span data-stu-id="b0758-140">List of Scope Tags for this Entity instance.</span></span> <span data-ttu-id="b0758-141">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-141">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-142">id</span><span class="sxs-lookup"><span data-stu-id="b0758-142">id</span></span>|<span data-ttu-id="b0758-143">文字列</span><span class="sxs-lookup"><span data-stu-id="b0758-143">String</span></span>|<span data-ttu-id="b0758-144">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="b0758-144">Key of the entity.</span></span> <span data-ttu-id="b0758-145">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-145">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-146">version</span><span class="sxs-lookup"><span data-stu-id="b0758-146">version</span></span>|<span data-ttu-id="b0758-147">String</span><span class="sxs-lookup"><span data-stu-id="b0758-147">String</span></span>|<span data-ttu-id="b0758-148">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="b0758-148">Version of the entity.</span></span> <span data-ttu-id="b0758-149">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="b0758-149">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="b0758-150">customSettings</span><span class="sxs-lookup"><span data-stu-id="b0758-150">customSettings</span></span>|<span data-ttu-id="b0758-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="b0758-151">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="b0758-152">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="b0758-152">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="b0758-153">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="b0758-153">Relationships</span></span>
<span data-ttu-id="b0758-154">なし</span><span class="sxs-lookup"><span data-stu-id="b0758-154">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="b0758-155">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="b0758-155">JSON Representation</span></span>
<span data-ttu-id="b0758-156">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="b0758-156">Here is a JSON representation of the resource.</span></span>
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




