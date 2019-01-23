---
title: dataSharingConsent リソースの種類
description: データの共有についてを同意するものとします。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: bf77a252c323ce83c2dcda44ac294161a4fd4747
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29425695"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="5c0c1-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="5c0c1-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="5c0c1-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="5c0c1-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5c0c1-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="5c0c1-107">データの共有についてを同意するものとします。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-107">Data sharing consent information.</span></span>

## <a name="methods"></a><span data-ttu-id="5c0c1-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c0c1-108">Methods</span></span>
|<span data-ttu-id="5c0c1-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="5c0c1-109">Method</span></span>|<span data-ttu-id="5c0c1-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="5c0c1-110">Return Type</span></span>|<span data-ttu-id="5c0c1-111">説明</span><span class="sxs-lookup"><span data-stu-id="5c0c1-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="5c0c1-112">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="5c0c1-112">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="5c0c1-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="5c0c1-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="5c0c1-114">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-114">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="5c0c1-115">DataSharingConsent を取得します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-115">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="5c0c1-116">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="5c0c1-116">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="5c0c1-117">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-117">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="5c0c1-118">DataSharingConsent を作成します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-118">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="5c0c1-119">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="5c0c1-119">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="5c0c1-120">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-120">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="5c0c1-121">DataSharingConsent を削除します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-121">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="5c0c1-122">なし</span><span class="sxs-lookup"><span data-stu-id="5c0c1-122">None</span></span>|<span data-ttu-id="5c0c1-123">の[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-123">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="5c0c1-124">DataSharingConsent を更新します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-124">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="5c0c1-125">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="5c0c1-125">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="5c0c1-126">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-126">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="5c0c1-127">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="5c0c1-127">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="5c0c1-128">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="5c0c1-128">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="5c0c1-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="5c0c1-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="5c0c1-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c0c1-130">Properties</span></span>
|<span data-ttu-id="5c0c1-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5c0c1-131">Property</span></span>|<span data-ttu-id="5c0c1-132">型</span><span class="sxs-lookup"><span data-stu-id="5c0c1-132">Type</span></span>|<span data-ttu-id="5c0c1-133">説明</span><span class="sxs-lookup"><span data-stu-id="5c0c1-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5c0c1-134">id</span><span class="sxs-lookup"><span data-stu-id="5c0c1-134">id</span></span>|<span data-ttu-id="5c0c1-135">String</span><span class="sxs-lookup"><span data-stu-id="5c0c1-135">String</span></span>|<span data-ttu-id="5c0c1-136">データ共有同意 Id</span><span class="sxs-lookup"><span data-stu-id="5c0c1-136">The data sharing consent Id</span></span>|
|<span data-ttu-id="5c0c1-137">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="5c0c1-137">serviceDisplayName</span></span>|<span data-ttu-id="5c0c1-138">String</span><span class="sxs-lookup"><span data-stu-id="5c0c1-138">String</span></span>|<span data-ttu-id="5c0c1-139">サービス作業の流れの表示名</span><span class="sxs-lookup"><span data-stu-id="5c0c1-139">The display name of the service work flow</span></span>|
|<span data-ttu-id="5c0c1-140">termsUrl</span><span class="sxs-lookup"><span data-stu-id="5c0c1-140">termsUrl</span></span>|<span data-ttu-id="5c0c1-141">String</span><span class="sxs-lookup"><span data-stu-id="5c0c1-141">String</span></span>|<span data-ttu-id="5c0c1-142">同意の共有データの TermsUrl</span><span class="sxs-lookup"><span data-stu-id="5c0c1-142">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="5c0c1-143">付与</span><span class="sxs-lookup"><span data-stu-id="5c0c1-143">granted</span></span>|<span data-ttu-id="5c0c1-144">Boolean</span><span class="sxs-lookup"><span data-stu-id="5c0c1-144">Boolean</span></span>|<span data-ttu-id="5c0c1-145">同意の共有データに付与されている状態</span><span class="sxs-lookup"><span data-stu-id="5c0c1-145">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="5c0c1-146">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="5c0c1-146">grantDateTime</span></span>|<span data-ttu-id="5c0c1-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="5c0c1-147">DateTimeOffset</span></span>|<span data-ttu-id="5c0c1-148">同意は、このアカウントに与えられました。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-148">The time consent was granted for this account</span></span>|
|<span data-ttu-id="5c0c1-149">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="5c0c1-149">grantedByUpn</span></span>|<span data-ttu-id="5c0c1-150">String</span><span class="sxs-lookup"><span data-stu-id="5c0c1-150">String</span></span>|<span data-ttu-id="5c0c1-151">このアカウントに許可を付与するユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="5c0c1-151">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="5c0c1-152">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="5c0c1-152">grantedByUserId</span></span>|<span data-ttu-id="5c0c1-153">String</span><span class="sxs-lookup"><span data-stu-id="5c0c1-153">String</span></span>|<span data-ttu-id="5c0c1-154">このアカウントに許可を付与するユーザーのユーザー Id</span><span class="sxs-lookup"><span data-stu-id="5c0c1-154">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="5c0c1-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="5c0c1-155">Relationships</span></span>
<span data-ttu-id="5c0c1-156">なし</span><span class="sxs-lookup"><span data-stu-id="5c0c1-156">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="5c0c1-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="5c0c1-157">JSON Representation</span></span>
<span data-ttu-id="5c0c1-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="5c0c1-158">Here is a JSON representation of the resource.</span></span>
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




