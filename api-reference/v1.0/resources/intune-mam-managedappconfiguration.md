---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: resourcePageType
ms.openlocfilehash: 86e1e5a2a768a9356ae580c4ceb01360a243c5cf
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36038032"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="2f9c6-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="2f9c6-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="2f9c6-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="2f9c6-105">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>


<span data-ttu-id="2f9c6-106">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="2f9c6-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="2f9c6-107">Methods</span></span>
|<span data-ttu-id="2f9c6-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="2f9c6-108">Method</span></span>|<span data-ttu-id="2f9c6-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="2f9c6-109">Return Type</span></span>|<span data-ttu-id="2f9c6-110">説明</span><span class="sxs-lookup"><span data-stu-id="2f9c6-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="2f9c6-111">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="2f9c6-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="2f9c6-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2f9c6-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="2f9c6-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="2f9c6-114">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="2f9c6-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="2f9c6-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="2f9c6-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="2f9c6-116">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="2f9c6-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f9c6-117">Properties</span></span>
|<span data-ttu-id="2f9c6-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="2f9c6-118">Property</span></span>|<span data-ttu-id="2f9c6-119">型</span><span class="sxs-lookup"><span data-stu-id="2f9c6-119">Type</span></span>|<span data-ttu-id="2f9c6-120">説明</span><span class="sxs-lookup"><span data-stu-id="2f9c6-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="2f9c6-121">displayName</span><span class="sxs-lookup"><span data-stu-id="2f9c6-121">displayName</span></span>|<span data-ttu-id="2f9c6-122">String</span><span class="sxs-lookup"><span data-stu-id="2f9c6-122">String</span></span>|<span data-ttu-id="2f9c6-123">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-123">Policy display name.</span></span> <span data-ttu-id="2f9c6-124">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-125">description</span><span class="sxs-lookup"><span data-stu-id="2f9c6-125">description</span></span>|<span data-ttu-id="2f9c6-126">String</span><span class="sxs-lookup"><span data-stu-id="2f9c6-126">String</span></span>|<span data-ttu-id="2f9c6-127">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-127">The policy's description.</span></span> <span data-ttu-id="2f9c6-128">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9c6-129">createdDateTime</span></span>|<span data-ttu-id="2f9c6-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9c6-130">DateTimeOffset</span></span>|<span data-ttu-id="2f9c6-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-131">The date and time the policy was created.</span></span> <span data-ttu-id="2f9c6-132">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="2f9c6-133">lastModifiedDateTime</span></span>|<span data-ttu-id="2f9c6-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="2f9c6-134">DateTimeOffset</span></span>|<span data-ttu-id="2f9c6-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-135">Last time the policy was modified.</span></span> <span data-ttu-id="2f9c6-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-137">id</span><span class="sxs-lookup"><span data-stu-id="2f9c6-137">id</span></span>|<span data-ttu-id="2f9c6-138">文字列</span><span class="sxs-lookup"><span data-stu-id="2f9c6-138">String</span></span>|<span data-ttu-id="2f9c6-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-139">Key of the entity.</span></span> <span data-ttu-id="2f9c6-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-141">version</span><span class="sxs-lookup"><span data-stu-id="2f9c6-141">version</span></span>|<span data-ttu-id="2f9c6-142">String</span><span class="sxs-lookup"><span data-stu-id="2f9c6-142">String</span></span>|<span data-ttu-id="2f9c6-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-143">Version of the entity.</span></span> <span data-ttu-id="2f9c6-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="2f9c6-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="2f9c6-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="2f9c6-145">customSettings</span></span>|<span data-ttu-id="2f9c6-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="2f9c6-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="2f9c6-147">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="2f9c6-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="2f9c6-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="2f9c6-148">Relationships</span></span>
<span data-ttu-id="2f9c6-149">なし</span><span class="sxs-lookup"><span data-stu-id="2f9c6-149">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="2f9c6-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="2f9c6-150">JSON Representation</span></span>
<span data-ttu-id="2f9c6-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="2f9c6-151">Here is a JSON representation of the resource.</span></span>
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



