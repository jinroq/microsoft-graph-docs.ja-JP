---
title: windowsInformationProtectionNetworkLearningSummary の更新
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 05c59d3bc28f5a0c29a33f1a0046b18331f46570
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29409224"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="a5f57-103">windowsInformationProtectionNetworkLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="a5f57-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="a5f57-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="a5f57-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="a5f57-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5f57-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="a5f57-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="a5f57-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="a5f57-107">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="a5f57-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="a5f57-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="a5f57-108">Prerequisites</span></span>
<span data-ttu-id="a5f57-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="a5f57-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="a5f57-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="a5f57-111">Permission type</span></span>|<span data-ttu-id="a5f57-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="a5f57-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="a5f57-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="a5f57-113">Delegated (work or school account)</span></span>|<span data-ttu-id="a5f57-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="a5f57-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="a5f57-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="a5f57-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="a5f57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5f57-116">Not supported.</span></span>|
|<span data-ttu-id="a5f57-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="a5f57-117">Application</span></span>|<span data-ttu-id="a5f57-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="a5f57-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="a5f57-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="a5f57-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="a5f57-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5f57-120">Request headers</span></span>
|<span data-ttu-id="a5f57-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="a5f57-121">Header</span></span>|<span data-ttu-id="a5f57-122">値</span><span class="sxs-lookup"><span data-stu-id="a5f57-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="a5f57-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="a5f57-123">Authorization</span></span>|<span data-ttu-id="a5f57-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="a5f57-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="a5f57-125">Accept</span><span class="sxs-lookup"><span data-stu-id="a5f57-125">Accept</span></span>|<span data-ttu-id="a5f57-126">application/json</span><span class="sxs-lookup"><span data-stu-id="a5f57-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="a5f57-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="a5f57-127">Request body</span></span>
<span data-ttu-id="a5f57-128">要求本文で、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="a5f57-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="a5f57-129">次の表に、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="a5f57-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="a5f57-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="a5f57-130">Property</span></span>|<span data-ttu-id="a5f57-131">型</span><span class="sxs-lookup"><span data-stu-id="a5f57-131">Type</span></span>|<span data-ttu-id="a5f57-132">説明</span><span class="sxs-lookup"><span data-stu-id="a5f57-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="a5f57-133">id</span><span class="sxs-lookup"><span data-stu-id="a5f57-133">id</span></span>|<span data-ttu-id="a5f57-134">String</span><span class="sxs-lookup"><span data-stu-id="a5f57-134">String</span></span>|<span data-ttu-id="a5f57-135">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="a5f57-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="a5f57-136">url</span><span class="sxs-lookup"><span data-stu-id="a5f57-136">url</span></span>|<span data-ttu-id="a5f57-137">String</span><span class="sxs-lookup"><span data-stu-id="a5f57-137">String</span></span>|<span data-ttu-id="a5f57-138">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="a5f57-138">Website url</span></span>|
|<span data-ttu-id="a5f57-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="a5f57-139">deviceCount</span></span>|<span data-ttu-id="a5f57-140">Int32</span><span class="sxs-lookup"><span data-stu-id="a5f57-140">Int32</span></span>|<span data-ttu-id="a5f57-141">デバイス数</span><span class="sxs-lookup"><span data-stu-id="a5f57-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="a5f57-142">応答</span><span class="sxs-lookup"><span data-stu-id="a5f57-142">Response</span></span>
<span data-ttu-id="a5f57-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="a5f57-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="a5f57-144">例</span><span class="sxs-lookup"><span data-stu-id="a5f57-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="a5f57-145">要求</span><span class="sxs-lookup"><span data-stu-id="a5f57-145">Request</span></span>
<span data-ttu-id="a5f57-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="a5f57-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="a5f57-147">応答</span><span class="sxs-lookup"><span data-stu-id="a5f57-147">Response</span></span>
<span data-ttu-id="a5f57-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="a5f57-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




