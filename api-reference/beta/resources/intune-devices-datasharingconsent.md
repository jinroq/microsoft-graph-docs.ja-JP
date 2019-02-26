---
title: dataSharingConsent リソースの種類
description: データ共有の同意情報。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 75ef8b899c6fa7645b31cd77ada7420b0f753a60
ms.sourcegitcommit: 03421b75d717101a499e0b311890f5714056e29e
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 02/21/2019
ms.locfileid: "30174651"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="d2ee1-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2ee1-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="d2ee1-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2ee1-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2ee1-106">データ共有の同意情報。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-106">Data sharing consent information.</span></span>

## <a name="methods"></a><span data-ttu-id="d2ee1-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2ee1-107">Methods</span></span>
|<span data-ttu-id="d2ee1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2ee1-108">Method</span></span>|<span data-ttu-id="d2ee1-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2ee1-109">Return Type</span></span>|<span data-ttu-id="d2ee1-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2ee1-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2ee1-111">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="d2ee1-111">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="d2ee1-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2ee1-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="d2ee1-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-113">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="d2ee1-114">dataSharingConsent を取得する</span><span class="sxs-lookup"><span data-stu-id="d2ee1-114">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="d2ee1-115">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2ee1-115">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2ee1-116">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-116">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2ee1-117">dataSharingConsent を作成する</span><span class="sxs-lookup"><span data-stu-id="d2ee1-117">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="d2ee1-118">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2ee1-118">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2ee1-119">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-119">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2ee1-120">dataSharingConsent の削除</span><span class="sxs-lookup"><span data-stu-id="d2ee1-120">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="d2ee1-121">なし</span><span class="sxs-lookup"><span data-stu-id="d2ee1-121">None</span></span>|<span data-ttu-id="d2ee1-122">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-122">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="d2ee1-123">dataSharingConsent の更新</span><span class="sxs-lookup"><span data-stu-id="d2ee1-123">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="d2ee1-124">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2ee1-124">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2ee1-125">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-125">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2ee1-126">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="d2ee1-126">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="d2ee1-127">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2ee1-127">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2ee1-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2ee1-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d2ee1-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2ee1-129">Properties</span></span>
|<span data-ttu-id="d2ee1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2ee1-130">Property</span></span>|<span data-ttu-id="d2ee1-131">型</span><span class="sxs-lookup"><span data-stu-id="d2ee1-131">Type</span></span>|<span data-ttu-id="d2ee1-132">説明</span><span class="sxs-lookup"><span data-stu-id="d2ee1-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2ee1-133">id</span><span class="sxs-lookup"><span data-stu-id="d2ee1-133">id</span></span>|<span data-ttu-id="d2ee1-134">String</span><span class="sxs-lookup"><span data-stu-id="d2ee1-134">String</span></span>|<span data-ttu-id="d2ee1-135">データ共有の同意 Id</span><span class="sxs-lookup"><span data-stu-id="d2ee1-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="d2ee1-136">servicedisplayname</span><span class="sxs-lookup"><span data-stu-id="d2ee1-136">serviceDisplayName</span></span>|<span data-ttu-id="d2ee1-137">String</span><span class="sxs-lookup"><span data-stu-id="d2ee1-137">String</span></span>|<span data-ttu-id="d2ee1-138">サービスワークフローの表示名</span><span class="sxs-lookup"><span data-stu-id="d2ee1-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="d2ee1-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="d2ee1-139">termsUrl</span></span>|<span data-ttu-id="d2ee1-140">String</span><span class="sxs-lookup"><span data-stu-id="d2ee1-140">String</span></span>|<span data-ttu-id="d2ee1-141">データ共有の同意の TermsUrl</span><span class="sxs-lookup"><span data-stu-id="d2ee1-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="d2ee1-142">granted</span><span class="sxs-lookup"><span data-stu-id="d2ee1-142">granted</span></span>|<span data-ttu-id="d2ee1-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2ee1-143">Boolean</span></span>|<span data-ttu-id="d2ee1-144">データ共有の同意の付与された状態</span><span class="sxs-lookup"><span data-stu-id="d2ee1-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="d2ee1-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="d2ee1-145">grantDateTime</span></span>|<span data-ttu-id="d2ee1-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2ee1-146">DateTimeOffset</span></span>|<span data-ttu-id="d2ee1-147">このアカウントに対して同意が与えられた時間</span><span class="sxs-lookup"><span data-stu-id="d2ee1-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="d2ee1-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="d2ee1-148">grantedByUpn</span></span>|<span data-ttu-id="d2ee1-149">String</span><span class="sxs-lookup"><span data-stu-id="d2ee1-149">String</span></span>|<span data-ttu-id="d2ee1-150">このアカウントに同意を付与したユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="d2ee1-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="d2ee1-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="d2ee1-151">grantedByUserId</span></span>|<span data-ttu-id="d2ee1-152">String</span><span class="sxs-lookup"><span data-stu-id="d2ee1-152">String</span></span>|<span data-ttu-id="d2ee1-153">このアカウントに同意を付与したユーザーの UserId</span><span class="sxs-lookup"><span data-stu-id="d2ee1-153">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2ee1-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2ee1-154">Relationships</span></span>
<span data-ttu-id="d2ee1-155">なし</span><span class="sxs-lookup"><span data-stu-id="d2ee1-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2ee1-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2ee1-156">JSON Representation</span></span>
<span data-ttu-id="d2ee1-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2ee1-157">Here is a JSON representation of the resource.</span></span>
<!-- {
  "blockType": "resource",
  "keyProperty": "id",
  "@odata.type": "microsoft.graph.dataSharingConsent"
}
-->
``` json
{
  "@odata.type": "#microsoft.graph.dataSharingConsent",
  "id": "String (identifier)",
  "serviceDisplayName": "String",
  "termsUrl": "String",
  "granted": true,
  "grantDateTime": "String (timestamp)",
  "grantedByUpn": "String",
  "grantedByUserId": "String"
}
```




