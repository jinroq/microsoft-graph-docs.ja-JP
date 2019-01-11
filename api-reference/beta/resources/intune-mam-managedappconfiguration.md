---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: 557a314893faeb268ae21d13ec78a46bff9d6e0f
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27809640"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="e45ff-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="e45ff-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="e45ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="e45ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e45ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e45ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="e45ff-107">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="e45ff-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="e45ff-108">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="e45ff-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="e45ff-109">Methods</span></span>
|<span data-ttu-id="e45ff-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="e45ff-110">Method</span></span>|<span data-ttu-id="e45ff-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="e45ff-111">Return Type</span></span>|<span data-ttu-id="e45ff-112">説明</span><span class="sxs-lookup"><span data-stu-id="e45ff-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="e45ff-113">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="e45ff-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="e45ff-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e45ff-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="e45ff-115">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="e45ff-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="e45ff-116">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="e45ff-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="e45ff-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="e45ff-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="e45ff-118">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="e45ff-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="e45ff-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e45ff-119">Properties</span></span>
|<span data-ttu-id="e45ff-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e45ff-120">Property</span></span>|<span data-ttu-id="e45ff-121">種類</span><span class="sxs-lookup"><span data-stu-id="e45ff-121">Type</span></span>|<span data-ttu-id="e45ff-122">説明</span><span class="sxs-lookup"><span data-stu-id="e45ff-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e45ff-123">displayName</span><span class="sxs-lookup"><span data-stu-id="e45ff-123">displayName</span></span>|<span data-ttu-id="e45ff-124">String</span><span class="sxs-lookup"><span data-stu-id="e45ff-124">String</span></span>|<span data-ttu-id="e45ff-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="e45ff-125">Policy display name.</span></span> <span data-ttu-id="e45ff-126">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-127">説明</span><span class="sxs-lookup"><span data-stu-id="e45ff-127">description</span></span>|<span data-ttu-id="e45ff-128">String</span><span class="sxs-lookup"><span data-stu-id="e45ff-128">String</span></span>|<span data-ttu-id="e45ff-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="e45ff-129">The policy's description.</span></span> <span data-ttu-id="e45ff-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="e45ff-131">createdDateTime</span></span>|<span data-ttu-id="e45ff-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45ff-132">DateTimeOffset</span></span>|<span data-ttu-id="e45ff-133">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="e45ff-133">The date and time the policy was created.</span></span> <span data-ttu-id="e45ff-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="e45ff-135">lastModifiedDateTime</span></span>|<span data-ttu-id="e45ff-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="e45ff-136">DateTimeOffset</span></span>|<span data-ttu-id="e45ff-137">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="e45ff-137">Last time the policy was modified.</span></span> <span data-ttu-id="e45ff-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-139">id</span><span class="sxs-lookup"><span data-stu-id="e45ff-139">id</span></span>|<span data-ttu-id="e45ff-140">String</span><span class="sxs-lookup"><span data-stu-id="e45ff-140">String</span></span>|<span data-ttu-id="e45ff-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="e45ff-141">Key of the entity.</span></span> <span data-ttu-id="e45ff-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-143">version</span><span class="sxs-lookup"><span data-stu-id="e45ff-143">version</span></span>|<span data-ttu-id="e45ff-144">String</span><span class="sxs-lookup"><span data-stu-id="e45ff-144">String</span></span>|<span data-ttu-id="e45ff-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="e45ff-145">Version of the entity.</span></span> <span data-ttu-id="e45ff-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="e45ff-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="e45ff-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="e45ff-147">customSettings</span></span>|<span data-ttu-id="e45ff-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="e45ff-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="e45ff-149">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="e45ff-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="e45ff-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="e45ff-150">Relationships</span></span>
<span data-ttu-id="e45ff-151">なし</span><span class="sxs-lookup"><span data-stu-id="e45ff-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="e45ff-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="e45ff-152">JSON Representation</span></span>
<span data-ttu-id="e45ff-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="e45ff-153">Here is a JSON representation of the resource.</span></span>
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





