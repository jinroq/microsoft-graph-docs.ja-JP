---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 5571a1c4b3f115280499ead992758a8ff46b2f26
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27963669"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="861b4-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="861b4-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="861b4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="861b4-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="861b4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="861b4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="861b4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="861b4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="861b4-107">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="861b4-107">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="861b4-108">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-108">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="861b4-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="861b4-109">Methods</span></span>
|<span data-ttu-id="861b4-110">メソッド</span><span class="sxs-lookup"><span data-stu-id="861b4-110">Method</span></span>|<span data-ttu-id="861b4-111">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="861b4-111">Return Type</span></span>|<span data-ttu-id="861b4-112">説明</span><span class="sxs-lookup"><span data-stu-id="861b4-112">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="861b4-113">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="861b4-113">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="861b4-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="861b4-114">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="861b4-115">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="861b4-115">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="861b4-116">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="861b4-116">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="861b4-117">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="861b4-117">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="861b4-118">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="861b4-118">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="861b4-119">プロパティ</span><span class="sxs-lookup"><span data-stu-id="861b4-119">Properties</span></span>
|<span data-ttu-id="861b4-120">プロパティ</span><span class="sxs-lookup"><span data-stu-id="861b4-120">Property</span></span>|<span data-ttu-id="861b4-121">種類</span><span class="sxs-lookup"><span data-stu-id="861b4-121">Type</span></span>|<span data-ttu-id="861b4-122">説明</span><span class="sxs-lookup"><span data-stu-id="861b4-122">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="861b4-123">displayName</span><span class="sxs-lookup"><span data-stu-id="861b4-123">displayName</span></span>|<span data-ttu-id="861b4-124">String</span><span class="sxs-lookup"><span data-stu-id="861b4-124">String</span></span>|<span data-ttu-id="861b4-125">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="861b4-125">Policy display name.</span></span> <span data-ttu-id="861b4-126">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-126">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-127">説明</span><span class="sxs-lookup"><span data-stu-id="861b4-127">description</span></span>|<span data-ttu-id="861b4-128">String</span><span class="sxs-lookup"><span data-stu-id="861b4-128">String</span></span>|<span data-ttu-id="861b4-129">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="861b4-129">The policy's description.</span></span> <span data-ttu-id="861b4-130">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-130">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-131">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="861b4-131">createdDateTime</span></span>|<span data-ttu-id="861b4-132">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861b4-132">DateTimeOffset</span></span>|<span data-ttu-id="861b4-133">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="861b4-133">The date and time the policy was created.</span></span> <span data-ttu-id="861b4-134">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-134">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-135">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="861b4-135">lastModifiedDateTime</span></span>|<span data-ttu-id="861b4-136">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="861b4-136">DateTimeOffset</span></span>|<span data-ttu-id="861b4-137">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="861b4-137">Last time the policy was modified.</span></span> <span data-ttu-id="861b4-138">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-138">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-139">id</span><span class="sxs-lookup"><span data-stu-id="861b4-139">id</span></span>|<span data-ttu-id="861b4-140">String</span><span class="sxs-lookup"><span data-stu-id="861b4-140">String</span></span>|<span data-ttu-id="861b4-141">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="861b4-141">Key of the entity.</span></span> <span data-ttu-id="861b4-142">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-142">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-143">version</span><span class="sxs-lookup"><span data-stu-id="861b4-143">version</span></span>|<span data-ttu-id="861b4-144">String</span><span class="sxs-lookup"><span data-stu-id="861b4-144">String</span></span>|<span data-ttu-id="861b4-145">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="861b4-145">Version of the entity.</span></span> <span data-ttu-id="861b4-146">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="861b4-146">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="861b4-147">customSettings</span><span class="sxs-lookup"><span data-stu-id="861b4-147">customSettings</span></span>|<span data-ttu-id="861b4-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="861b4-148">[keyValuePair](../resources/intune-shared-keyvaluepair.md) collection</span></span>|<span data-ttu-id="861b4-149">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="861b4-149">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="861b4-150">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="861b4-150">Relationships</span></span>
<span data-ttu-id="861b4-151">なし</span><span class="sxs-lookup"><span data-stu-id="861b4-151">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="861b4-152">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="861b4-152">JSON Representation</span></span>
<span data-ttu-id="861b4-153">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="861b4-153">Here is a JSON representation of the resource.</span></span>
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





