---
title: dataSharingConsent リソースの種類
description: データの共有についてを同意するものとします。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: 75d4582d1ad7503757dda4887ccff30149f70af8
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27962388"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="39428-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="39428-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="39428-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="39428-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="39428-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="39428-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="39428-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="39428-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="39428-107">データの共有についてを同意するものとします。</span><span class="sxs-lookup"><span data-stu-id="39428-107">Data sharing consent information.</span></span>
## <a name="methods"></a><span data-ttu-id="39428-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="39428-108">Methods</span></span>
|<span data-ttu-id="39428-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="39428-109">Method</span></span>|<span data-ttu-id="39428-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="39428-110">Return Type</span></span>|<span data-ttu-id="39428-111">説明</span><span class="sxs-lookup"><span data-stu-id="39428-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="39428-112">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="39428-112">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="39428-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="39428-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="39428-114">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="39428-114">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="39428-115">DataSharingConsent を取得します。</span><span class="sxs-lookup"><span data-stu-id="39428-115">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="39428-116">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="39428-116">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="39428-117">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="39428-117">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="39428-118">DataSharingConsent を作成します。</span><span class="sxs-lookup"><span data-stu-id="39428-118">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="39428-119">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="39428-119">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="39428-120">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="39428-120">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="39428-121">DataSharingConsent を削除します。</span><span class="sxs-lookup"><span data-stu-id="39428-121">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="39428-122">なし</span><span class="sxs-lookup"><span data-stu-id="39428-122">None</span></span>|<span data-ttu-id="39428-123">の[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="39428-123">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="39428-124">DataSharingConsent を更新します。</span><span class="sxs-lookup"><span data-stu-id="39428-124">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="39428-125">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="39428-125">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="39428-126">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="39428-126">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="39428-127">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="39428-127">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="39428-128">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="39428-128">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="39428-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="39428-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="39428-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39428-130">Properties</span></span>
|<span data-ttu-id="39428-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="39428-131">Property</span></span>|<span data-ttu-id="39428-132">種類</span><span class="sxs-lookup"><span data-stu-id="39428-132">Type</span></span>|<span data-ttu-id="39428-133">説明</span><span class="sxs-lookup"><span data-stu-id="39428-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="39428-134">ID</span><span class="sxs-lookup"><span data-stu-id="39428-134">id</span></span>|<span data-ttu-id="39428-135">String</span><span class="sxs-lookup"><span data-stu-id="39428-135">String</span></span>|<span data-ttu-id="39428-136">データ共有同意 Id</span><span class="sxs-lookup"><span data-stu-id="39428-136">The data sharing consent Id</span></span>|
|<span data-ttu-id="39428-137">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="39428-137">serviceDisplayName</span></span>|<span data-ttu-id="39428-138">String</span><span class="sxs-lookup"><span data-stu-id="39428-138">String</span></span>|<span data-ttu-id="39428-139">サービス作業の流れの表示名</span><span class="sxs-lookup"><span data-stu-id="39428-139">The display name of the service work flow</span></span>|
|<span data-ttu-id="39428-140">termsUrl</span><span class="sxs-lookup"><span data-stu-id="39428-140">termsUrl</span></span>|<span data-ttu-id="39428-141">String</span><span class="sxs-lookup"><span data-stu-id="39428-141">String</span></span>|<span data-ttu-id="39428-142">同意の共有データの TermsUrl</span><span class="sxs-lookup"><span data-stu-id="39428-142">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="39428-143">付与</span><span class="sxs-lookup"><span data-stu-id="39428-143">granted</span></span>|<span data-ttu-id="39428-144">ブール型</span><span class="sxs-lookup"><span data-stu-id="39428-144">Boolean</span></span>|<span data-ttu-id="39428-145">同意の共有データに付与されている状態</span><span class="sxs-lookup"><span data-stu-id="39428-145">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="39428-146">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="39428-146">grantDateTime</span></span>|<span data-ttu-id="39428-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="39428-147">DateTimeOffset</span></span>|<span data-ttu-id="39428-148">同意は、このアカウントに与えられました。</span><span class="sxs-lookup"><span data-stu-id="39428-148">The time consent was granted for this account</span></span>|
|<span data-ttu-id="39428-149">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="39428-149">grantedByUpn</span></span>|<span data-ttu-id="39428-150">String</span><span class="sxs-lookup"><span data-stu-id="39428-150">String</span></span>|<span data-ttu-id="39428-151">このアカウントに許可を付与するユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="39428-151">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="39428-152">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="39428-152">grantedByUserId</span></span>|<span data-ttu-id="39428-153">String</span><span class="sxs-lookup"><span data-stu-id="39428-153">String</span></span>|<span data-ttu-id="39428-154">このアカウントに許可を付与するユーザーのユーザー Id</span><span class="sxs-lookup"><span data-stu-id="39428-154">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="39428-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="39428-155">Relationships</span></span>
<span data-ttu-id="39428-156">なし</span><span class="sxs-lookup"><span data-stu-id="39428-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="39428-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="39428-157">JSON Representation</span></span>
<span data-ttu-id="39428-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="39428-158">Here is a JSON representation of the resource.</span></span>
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





