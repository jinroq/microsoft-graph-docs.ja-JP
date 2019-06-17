---
title: dataSharingConsent リソースの種類
description: データ共有の同意情報。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1a221b420199d801e084746ed058b3f6dc1f53bf
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34983189"
---
# <a name="datasharingconsent-resource-type"></a><span data-ttu-id="d2051-103">dataSharingConsent リソースの種類</span><span class="sxs-lookup"><span data-stu-id="d2051-103">dataSharingConsent resource type</span></span>

> <span data-ttu-id="d2051-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d2051-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d2051-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d2051-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d2051-106">データ共有の同意情報。</span><span class="sxs-lookup"><span data-stu-id="d2051-106">Data sharing consent information.</span></span>

## <a name="methods"></a><span data-ttu-id="d2051-107">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2051-107">Methods</span></span>
|<span data-ttu-id="d2051-108">メソッド</span><span class="sxs-lookup"><span data-stu-id="d2051-108">Method</span></span>|<span data-ttu-id="d2051-109">戻り値の型</span><span class="sxs-lookup"><span data-stu-id="d2051-109">Return Type</span></span>|<span data-ttu-id="d2051-110">説明</span><span class="sxs-lookup"><span data-stu-id="d2051-110">Description</span></span>|
|:---|:---|:---|
|[<span data-ttu-id="d2051-111">リスト dataSharingConsents</span><span class="sxs-lookup"><span data-stu-id="d2051-111">List dataSharingConsents</span></span>](../api/intune-devices-datasharingconsent-list.md)|<span data-ttu-id="d2051-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)コレクション</span><span class="sxs-lookup"><span data-stu-id="d2051-112">[dataSharingConsent](../resources/intune-devices-datasharingconsent.md) collection</span></span>|<span data-ttu-id="d2051-113">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップをリストします。</span><span class="sxs-lookup"><span data-stu-id="d2051-113">List properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) objects.</span></span>|
|[<span data-ttu-id="d2051-114">DataSharingConsent を取得する</span><span class="sxs-lookup"><span data-stu-id="d2051-114">Get dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-get.md)|[<span data-ttu-id="d2051-115">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2051-115">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2051-116">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティとリレーションシップを読み取ります。</span><span class="sxs-lookup"><span data-stu-id="d2051-116">Read properties and relationships of the [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2051-117">DataSharingConsent を作成する</span><span class="sxs-lookup"><span data-stu-id="d2051-117">Create dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-create.md)|[<span data-ttu-id="d2051-118">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2051-118">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2051-119">新しい[dataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="d2051-119">Create a new [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2051-120">DataSharingConsent の削除</span><span class="sxs-lookup"><span data-stu-id="d2051-120">Delete dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-delete.md)|<span data-ttu-id="d2051-121">None</span><span class="sxs-lookup"><span data-stu-id="d2051-121">None</span></span>|<span data-ttu-id="d2051-122">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="d2051-122">Deletes a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md).</span></span>|
|[<span data-ttu-id="d2051-123">DataSharingConsent の更新</span><span class="sxs-lookup"><span data-stu-id="d2051-123">Update dataSharingConsent</span></span>](../api/intune-devices-datasharingconsent-update.md)|[<span data-ttu-id="d2051-124">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2051-124">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2051-125">[DataSharingConsent](../resources/intune-devices-datasharingconsent.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d2051-125">Update the properties of a [dataSharingConsent](../resources/intune-devices-datasharingconsent.md) object.</span></span>|
|[<span data-ttu-id="d2051-126">consentToDataSharing アクション</span><span class="sxs-lookup"><span data-stu-id="d2051-126">consentToDataSharing action</span></span>](../api/intune-devices-datasharingconsent-consenttodatasharing.md)|[<span data-ttu-id="d2051-127">dataSharingConsent</span><span class="sxs-lookup"><span data-stu-id="d2051-127">dataSharingConsent</span></span>](../resources/intune-devices-datasharingconsent.md)|<span data-ttu-id="d2051-128">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="d2051-128">Not yet documented</span></span>|

## <a name="properties"></a><span data-ttu-id="d2051-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2051-129">Properties</span></span>
|<span data-ttu-id="d2051-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d2051-130">Property</span></span>|<span data-ttu-id="d2051-131">型</span><span class="sxs-lookup"><span data-stu-id="d2051-131">Type</span></span>|<span data-ttu-id="d2051-132">説明</span><span class="sxs-lookup"><span data-stu-id="d2051-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d2051-133">id</span><span class="sxs-lookup"><span data-stu-id="d2051-133">id</span></span>|<span data-ttu-id="d2051-134">String</span><span class="sxs-lookup"><span data-stu-id="d2051-134">String</span></span>|<span data-ttu-id="d2051-135">データ共有の同意 Id</span><span class="sxs-lookup"><span data-stu-id="d2051-135">The data sharing consent Id</span></span>|
|<span data-ttu-id="d2051-136">serviceDisplayName</span><span class="sxs-lookup"><span data-stu-id="d2051-136">serviceDisplayName</span></span>|<span data-ttu-id="d2051-137">String</span><span class="sxs-lookup"><span data-stu-id="d2051-137">String</span></span>|<span data-ttu-id="d2051-138">サービスワークフローの表示名</span><span class="sxs-lookup"><span data-stu-id="d2051-138">The display name of the service work flow</span></span>|
|<span data-ttu-id="d2051-139">termsUrl</span><span class="sxs-lookup"><span data-stu-id="d2051-139">termsUrl</span></span>|<span data-ttu-id="d2051-140">String</span><span class="sxs-lookup"><span data-stu-id="d2051-140">String</span></span>|<span data-ttu-id="d2051-141">データ共有の同意の TermsUrl</span><span class="sxs-lookup"><span data-stu-id="d2051-141">The TermsUrl for the data sharing consent</span></span>|
|<span data-ttu-id="d2051-142">granted</span><span class="sxs-lookup"><span data-stu-id="d2051-142">granted</span></span>|<span data-ttu-id="d2051-143">Boolean</span><span class="sxs-lookup"><span data-stu-id="d2051-143">Boolean</span></span>|<span data-ttu-id="d2051-144">データ共有の同意の付与された状態</span><span class="sxs-lookup"><span data-stu-id="d2051-144">The granted state for the data sharing consent</span></span>|
|<span data-ttu-id="d2051-145">grantDateTime</span><span class="sxs-lookup"><span data-stu-id="d2051-145">grantDateTime</span></span>|<span data-ttu-id="d2051-146">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="d2051-146">DateTimeOffset</span></span>|<span data-ttu-id="d2051-147">このアカウントに対して同意が与えられた時間</span><span class="sxs-lookup"><span data-stu-id="d2051-147">The time consent was granted for this account</span></span>|
|<span data-ttu-id="d2051-148">grantedByUpn</span><span class="sxs-lookup"><span data-stu-id="d2051-148">grantedByUpn</span></span>|<span data-ttu-id="d2051-149">String</span><span class="sxs-lookup"><span data-stu-id="d2051-149">String</span></span>|<span data-ttu-id="d2051-150">このアカウントに同意を付与したユーザーの Upn</span><span class="sxs-lookup"><span data-stu-id="d2051-150">The Upn of the user that granted consent for this account</span></span>|
|<span data-ttu-id="d2051-151">grantedByUserId</span><span class="sxs-lookup"><span data-stu-id="d2051-151">grantedByUserId</span></span>|<span data-ttu-id="d2051-152">String</span><span class="sxs-lookup"><span data-stu-id="d2051-152">String</span></span>|<span data-ttu-id="d2051-153">このアカウントに同意を付与したユーザーの UserId</span><span class="sxs-lookup"><span data-stu-id="d2051-153">The UserId of the user that granted consent for this account</span></span>|

## <a name="relationships"></a><span data-ttu-id="d2051-154">リレーションシップ</span><span class="sxs-lookup"><span data-stu-id="d2051-154">Relationships</span></span>
<span data-ttu-id="d2051-155">なし</span><span class="sxs-lookup"><span data-stu-id="d2051-155">None</span></span>

## <a name="json-representation"></a><span data-ttu-id="d2051-156">JSON 表記</span><span class="sxs-lookup"><span data-stu-id="d2051-156">JSON Representation</span></span>
<span data-ttu-id="d2051-157">以下は、リソースの JSON 表記です。</span><span class="sxs-lookup"><span data-stu-id="d2051-157">Here is a JSON representation of the resource.</span></span>
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





