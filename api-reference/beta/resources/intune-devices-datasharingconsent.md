---
title: dataSharingConsent リソースの種類
description: データの共有についてを同意するものとします。
author: tfitzmac
ms.openlocfilehash: 250ad388a5c619a6fd2753d172734145ea720776
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27342936"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="15c06-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="15c06-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="15c06-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="15c06-104">**Important:** APIs under the / beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="15c06-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="15c06-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="15c06-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="15c06-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="15c06-107">データの共有についてを同意するものとします。</span><span class="sxs-lookup"><span data-stu-id="15c06-107">Data sharing consent information.</span></span>
## <a name="methods"></a><span data-ttu-id="15c06-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="15c06-108">Methods</span></span>
|<span data-ttu-id="15c06-109">メソッド</span><span class="sxs-lookup"><span data-stu-id="15c06-109">Method</span></span>|<span data-ttu-id="15c06-110">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="15c06-110">Return Type</span></span>|<span data-ttu-id="15c06-111">説明</span><span class="sxs-lookup"><span data-stu-id="15c06-111">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="15c06-112">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="15c06-112">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="15c06-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="15c06-113">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="15c06-114">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を一覧表示します。</span><span class="sxs-lookup"><span data-stu-id="15c06-114">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="15c06-115">DataSharingConsent を取得します。</span><span class="sxs-lookup"><span data-stu-id="15c06-115">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="15c06-116">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="15c06-116">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="15c06-117">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティと関係を参照してください。</span><span class="sxs-lookup"><span data-stu-id="15c06-117">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="15c06-118">DataSharingConsent を作成します。</span><span class="sxs-lookup"><span data-stu-id="15c06-118">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="15c06-119">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="15c06-119">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="15c06-120">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="15c06-120">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="15c06-121">DataSharingConsent を削除します。</span><span class="sxs-lookup"><span data-stu-id="15c06-121">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="15c06-122">なし</span><span class="sxs-lookup"><span data-stu-id="15c06-122">None</span></span>|<span data-ttu-id="15c06-123">の[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="15c06-123">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="15c06-124">DataSharingConsent を更新します。</span><span class="sxs-lookup"><span data-stu-id="15c06-124">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="15c06-125">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="15c06-125">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="15c06-126">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="15c06-126">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="15c06-127">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="15c06-127">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="15c06-128">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="15c06-128">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="15c06-129">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="15c06-129">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="15c06-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15c06-130">Properties</span></span>
|<span data-ttu-id="15c06-131">プロパティ</span><span class="sxs-lookup"><span data-stu-id="15c06-131">Property</span></span>|<span data-ttu-id="15c06-132">種類</span><span class="sxs-lookup"><span data-stu-id="15c06-132">Type</span></span>|<span data-ttu-id="15c06-133">説明</span><span class="sxs-lookup"><span data-stu-id="15c06-133">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="15c06-134">ID</span><span class="sxs-lookup"><span data-stu-id="15c06-134">id</span></span>|<span data-ttu-id="15c06-135">String</span><span class="sxs-lookup"><span data-stu-id="15c06-135">String</span></span>|<span data-ttu-id="15c06-136">データ共有同意 Id</span><span class="sxs-lookup"><span data-stu-id="15c06-136">The data sharing consent Id</span></span>|
|<span data-ttu-id="15c06-137">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="15c06-137">serviceDisplayName</span></span>|<span data-ttu-id="15c06-138">String</span><span class="sxs-lookup"><span data-stu-id="15c06-138">String</span></span>|<span data-ttu-id="15c06-139">サービス作業の流れの表示名</span><span class="sxs-lookup"><span data-stu-id="15c06-139">The display name of the service work flow</span></span>|
|<span data-ttu-id="15c06-140">termsUrl</span><span class="sxs-lookup"><span data-stu-id="15c06-140">termsUrl</span></span>|<span data-ttu-id="15c06-141">String</span><span class="sxs-lookup"><span data-stu-id="15c06-141">String</span></span>|<span data-ttu-id="15c06-142">同意の共有データの TermsUrl</span><span class="sxs-lookup"><span data-stu-id="15c06-142">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="15c06-143">付与</span><span class="sxs-lookup"><span data-stu-id="15c06-143">granted</span></span>|<span data-ttu-id="15c06-144">ブール型</span><span class="sxs-lookup"><span data-stu-id="15c06-144">Boolean</span></span>|<span data-ttu-id="15c06-145">同意の共有データに付与されている状態</span><span class="sxs-lookup"><span data-stu-id="15c06-145">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="15c06-146">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="15c06-146">grantDateTime</span></span>|<span data-ttu-id="15c06-147">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="15c06-147">DateTimeOffset</span></span>|<span data-ttu-id="15c06-148">同意は、このアカウントに与えられました。</span><span class="sxs-lookup"><span data-stu-id="15c06-148">The time consent was granted for this account</span></span>|
|<span data-ttu-id="15c06-149">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="15c06-149">grantedByUpn</span></span>|<span data-ttu-id="15c06-150">String</span><span class="sxs-lookup"><span data-stu-id="15c06-150">String</span></span>|<span data-ttu-id="15c06-151">このアカウントに許可を付与するユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="15c06-151">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="15c06-152">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="15c06-152">grantedByUserId</span></span>|<span data-ttu-id="15c06-153">String</span><span class="sxs-lookup"><span data-stu-id="15c06-153">String</span></span>|<span data-ttu-id="15c06-154">このアカウントに許可を付与するユーザーのユーザー Id</span><span class="sxs-lookup"><span data-stu-id="15c06-154">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="15c06-155">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="15c06-155">Relationships</span></span>
<span data-ttu-id="15c06-156">なし</span><span class="sxs-lookup"><span data-stu-id="15c06-156">None</span></span>
## <a name="json-representation"></a><span data-ttu-id="15c06-157">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="15c06-157">JSON Representation</span></span>
<span data-ttu-id="15c06-158">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="15c06-158">Here is a JSON representation of the resource.</span></span>
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





