---
title: managedAppConfiguration リソースの種類
description: 構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。
author: tfitzmac
ms.openlocfilehash: e4b20c642f49b2f110ced2f72a5a54a6583b561f
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27346908"
---
# <a name="managedappconfiguration-resource-type"></a><span data-ttu-id="6cad3-103">managedAppConfiguration リソースの種類</span><span class="sxs-lookup"><span data-stu-id="6cad3-103">managedAppConfiguration resource type</span></span>

> <span data-ttu-id="6cad3-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="6cad3-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="6cad3-105">構成の対象であるユーザーに対して、一連のカスタム設定を現状のままアプリに配信するために使用する構成です。</span><span class="sxs-lookup"><span data-stu-id="6cad3-105">Configuration used to deliver a set of custom settings as-is to apps for users to whom the configuration is scoped</span></span>

<span data-ttu-id="6cad3-106">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-106">Inherits from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>

## <a name="methods"></a><span data-ttu-id="6cad3-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="6cad3-107">Methods</span></span>
|<span data-ttu-id="6cad3-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="6cad3-108">Method</span></span>|<span data-ttu-id="6cad3-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="6cad3-109">Return Type</span></span>|<span data-ttu-id="6cad3-110">説明</span><span class="sxs-lookup"><span data-stu-id="6cad3-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="6cad3-111">managedAppConfigurations のリスト</span><span class="sxs-lookup"><span data-stu-id="6cad3-111">List managedAppConfigurations</span></span>](../api/intune-mam-managedappconfiguration-list.md)|<span data-ttu-id="6cad3-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6cad3-112">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) collection</span></span>|<span data-ttu-id="6cad3-113">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="6cad3-113">List properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) objects.</span></span>|
|[<span data-ttu-id="6cad3-114">managedAppConfiguration の取得</span><span class="sxs-lookup"><span data-stu-id="6cad3-114">Get managedAppConfiguration</span></span>](../api/intune-mam-managedappconfiguration-get.md)|[<span data-ttu-id="6cad3-115">managedAppConfiguration</span><span class="sxs-lookup"><span data-stu-id="6cad3-115">managedAppConfiguration</span></span>](../resources/intune-mam-managedappconfiguration.md)|<span data-ttu-id="6cad3-116">[managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="6cad3-116">Read properties and relationships of the [managedAppConfiguration](../resources/intune-mam-managedappconfiguration.md) object.</span></span>|

## <a name="properties"></a><span data-ttu-id="6cad3-117">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cad3-117">Properties</span></span>
|<span data-ttu-id="6cad3-118">プロパティ</span><span class="sxs-lookup"><span data-stu-id="6cad3-118">Property</span></span>|<span data-ttu-id="6cad3-119">種類</span><span class="sxs-lookup"><span data-stu-id="6cad3-119">Type</span></span>|<span data-ttu-id="6cad3-120">説明</span><span class="sxs-lookup"><span data-stu-id="6cad3-120">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="6cad3-121">displayName</span><span class="sxs-lookup"><span data-stu-id="6cad3-121">displayName</span></span>|<span data-ttu-id="6cad3-122">String</span><span class="sxs-lookup"><span data-stu-id="6cad3-122">String</span></span>|<span data-ttu-id="6cad3-123">ポリシーの表示名。</span><span class="sxs-lookup"><span data-stu-id="6cad3-123">Policy display name.</span></span> <span data-ttu-id="6cad3-124">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-124">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-125">説明</span><span class="sxs-lookup"><span data-stu-id="6cad3-125">description</span></span>|<span data-ttu-id="6cad3-126">String</span><span class="sxs-lookup"><span data-stu-id="6cad3-126">String</span></span>|<span data-ttu-id="6cad3-127">ポリシーの説明。</span><span class="sxs-lookup"><span data-stu-id="6cad3-127">The policy's description.</span></span> <span data-ttu-id="6cad3-128">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-128">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-129">createdDateTime</span><span class="sxs-lookup"><span data-stu-id="6cad3-129">createdDateTime</span></span>|<span data-ttu-id="6cad3-130">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cad3-130">DateTimeOffset</span></span>|<span data-ttu-id="6cad3-131">ポリシーが作成された日時。</span><span class="sxs-lookup"><span data-stu-id="6cad3-131">The date and time the policy was created.</span></span> <span data-ttu-id="6cad3-132">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-132">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-133">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="6cad3-133">lastModifiedDateTime</span></span>|<span data-ttu-id="6cad3-134">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="6cad3-134">DateTimeOffset</span></span>|<span data-ttu-id="6cad3-135">ポリシーが変更された最終日時。</span><span class="sxs-lookup"><span data-stu-id="6cad3-135">Last time the policy was modified.</span></span> <span data-ttu-id="6cad3-136">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-136">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-137">id</span><span class="sxs-lookup"><span data-stu-id="6cad3-137">id</span></span>|<span data-ttu-id="6cad3-138">String</span><span class="sxs-lookup"><span data-stu-id="6cad3-138">String</span></span>|<span data-ttu-id="6cad3-139">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="6cad3-139">Key of the entity.</span></span> <span data-ttu-id="6cad3-140">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-140">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-141">version</span><span class="sxs-lookup"><span data-stu-id="6cad3-141">version</span></span>|<span data-ttu-id="6cad3-142">String</span><span class="sxs-lookup"><span data-stu-id="6cad3-142">String</span></span>|<span data-ttu-id="6cad3-143">エンティティのバージョン。</span><span class="sxs-lookup"><span data-stu-id="6cad3-143">Version of the entity.</span></span> <span data-ttu-id="6cad3-144">[managedAppPolicy](../resources/intune-mam-managedapppolicy.md) から継承します</span><span class="sxs-lookup"><span data-stu-id="6cad3-144">Inherited from [managedAppPolicy](../resources/intune-mam-managedapppolicy.md)</span></span>|
|<span data-ttu-id="6cad3-145">customSettings</span><span class="sxs-lookup"><span data-stu-id="6cad3-145">customSettings</span></span>|<span data-ttu-id="6cad3-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) コレクション</span><span class="sxs-lookup"><span data-stu-id="6cad3-146">[keyValuePair](../resources/intune-mam-keyvaluepair.md) collection</span></span>|<span data-ttu-id="6cad3-147">構成の対象であるユーザーに対して、このサービスで変更せずに、アプリに送信される文字列キーと文字列値の一連のペア</span><span class="sxs-lookup"><span data-stu-id="6cad3-147">A set of string key and string value pairs to be sent to apps for users to whom the configuration is scoped, unalterned by this service</span></span>|

## <a name="relationships"></a><span data-ttu-id="6cad3-148">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="6cad3-148">Relationships</span></span>
<span data-ttu-id="6cad3-149">なし</span><span class="sxs-lookup"><span data-stu-id="6cad3-149">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="6cad3-150">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="6cad3-150">JSON Representation</span></span>
<span data-ttu-id="6cad3-151">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="6cad3-151">Here is a JSON representation of the resource.</span></span>
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



