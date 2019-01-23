---
title: windowsInformationProtectionNetworkLearningSummary の作成
description: 新しい windowsInformationProtectionNetworkLearningSummary オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: ef10a71e9e6b59c86e1450cea8e40465bc0f70af
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29403253"
---
# <a name="create-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="54726-103">windowsInformationProtectionNetworkLearningSummary の作成</span><span class="sxs-lookup"><span data-stu-id="54726-103">Create windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="54726-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="54726-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="54726-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54726-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="54726-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="54726-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="54726-107">新しい [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="54726-107">Create a new [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="54726-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="54726-108">Prerequisites</span></span>
<span data-ttu-id="54726-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="54726-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="54726-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="54726-111">Permission type</span></span>|<span data-ttu-id="54726-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="54726-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="54726-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="54726-113">Delegated (work or school account)</span></span>|<span data-ttu-id="54726-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="54726-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="54726-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="54726-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="54726-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54726-116">Not supported.</span></span>|
|<span data-ttu-id="54726-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="54726-117">Application</span></span>|<span data-ttu-id="54726-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="54726-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="54726-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="54726-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/windowsInformationProtectionNetworkLearningSummaries
```

## <a name="request-headers"></a><span data-ttu-id="54726-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54726-120">Request headers</span></span>
|<span data-ttu-id="54726-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="54726-121">Header</span></span>|<span data-ttu-id="54726-122">値</span><span class="sxs-lookup"><span data-stu-id="54726-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="54726-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="54726-123">Authorization</span></span>|<span data-ttu-id="54726-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="54726-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="54726-125">Accept</span><span class="sxs-lookup"><span data-stu-id="54726-125">Accept</span></span>|<span data-ttu-id="54726-126">application/json</span><span class="sxs-lookup"><span data-stu-id="54726-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="54726-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="54726-127">Request body</span></span>
<span data-ttu-id="54726-128">要求本文で、windowsInformationProtectionNetworkLearningSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="54726-128">In the request body, supply a JSON representation for the windowsInformationProtectionNetworkLearningSummary object.</span></span>

<span data-ttu-id="54726-129">次の表に、windowsInformationProtectionNetworkLearningSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="54726-129">The following table shows the properties that are required when you create the windowsInformationProtectionNetworkLearningSummary.</span></span>

|<span data-ttu-id="54726-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="54726-130">Property</span></span>|<span data-ttu-id="54726-131">型</span><span class="sxs-lookup"><span data-stu-id="54726-131">Type</span></span>|<span data-ttu-id="54726-132">説明</span><span class="sxs-lookup"><span data-stu-id="54726-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="54726-133">id</span><span class="sxs-lookup"><span data-stu-id="54726-133">id</span></span>|<span data-ttu-id="54726-134">String</span><span class="sxs-lookup"><span data-stu-id="54726-134">String</span></span>|<span data-ttu-id="54726-135">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="54726-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="54726-136">url</span><span class="sxs-lookup"><span data-stu-id="54726-136">url</span></span>|<span data-ttu-id="54726-137">String</span><span class="sxs-lookup"><span data-stu-id="54726-137">String</span></span>|<span data-ttu-id="54726-138">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="54726-138">Website url</span></span>|
|<span data-ttu-id="54726-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="54726-139">deviceCount</span></span>|<span data-ttu-id="54726-140">Int32</span><span class="sxs-lookup"><span data-stu-id="54726-140">Int32</span></span>|<span data-ttu-id="54726-141">デバイス数</span><span class="sxs-lookup"><span data-stu-id="54726-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="54726-142">応答</span><span class="sxs-lookup"><span data-stu-id="54726-142">Response</span></span>
<span data-ttu-id="54726-143">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="54726-143">If successful, this method returns a `201 Created` response code and a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="54726-144">例</span><span class="sxs-lookup"><span data-stu-id="54726-144">Example</span></span>

### <a name="request"></a><span data-ttu-id="54726-145">要求</span><span class="sxs-lookup"><span data-stu-id="54726-145">Request</span></span>
<span data-ttu-id="54726-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="54726-146">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="54726-147">応答</span><span class="sxs-lookup"><span data-stu-id="54726-147">Response</span></span>
<span data-ttu-id="54726-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="54726-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 186

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "id": "242108f7-08f7-2421-f708-2124f7082124",
  "url": "Url value",
  "deviceCount": 11
}
```




