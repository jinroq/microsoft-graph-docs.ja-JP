---
title: windowsInformationProtectionNetworkLearningSummary の更新
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 335fee7e664000584fa4542985a3b014d827f0d9
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27344437"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="336ff-103">windowsInformationProtectionNetworkLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="336ff-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="336ff-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="336ff-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="336ff-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="336ff-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="336ff-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="336ff-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="336ff-107">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="336ff-107">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="336ff-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="336ff-108">Prerequisites</span></span>
<span data-ttu-id="336ff-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="336ff-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="336ff-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="336ff-111">Permission type</span></span>|<span data-ttu-id="336ff-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="336ff-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="336ff-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="336ff-113">Delegated (work or school account)</span></span>|<span data-ttu-id="336ff-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="336ff-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="336ff-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="336ff-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="336ff-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="336ff-116">Not supported.</span></span>|
|<span data-ttu-id="336ff-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="336ff-117">Application</span></span>|<span data-ttu-id="336ff-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="336ff-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="336ff-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="336ff-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="336ff-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="336ff-120">Request headers</span></span>
|<span data-ttu-id="336ff-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="336ff-121">Header</span></span>|<span data-ttu-id="336ff-122">値</span><span class="sxs-lookup"><span data-stu-id="336ff-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="336ff-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="336ff-123">Authorization</span></span>|<span data-ttu-id="336ff-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="336ff-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="336ff-125">Accept</span><span class="sxs-lookup"><span data-stu-id="336ff-125">Accept</span></span>|<span data-ttu-id="336ff-126">application/json</span><span class="sxs-lookup"><span data-stu-id="336ff-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="336ff-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="336ff-127">Request body</span></span>
<span data-ttu-id="336ff-128">要求本文で、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="336ff-128">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="336ff-129">次の表に、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="336ff-129">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="336ff-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="336ff-130">Property</span></span>|<span data-ttu-id="336ff-131">種類</span><span class="sxs-lookup"><span data-stu-id="336ff-131">Type</span></span>|<span data-ttu-id="336ff-132">説明</span><span class="sxs-lookup"><span data-stu-id="336ff-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="336ff-133">ID</span><span class="sxs-lookup"><span data-stu-id="336ff-133">id</span></span>|<span data-ttu-id="336ff-134">String</span><span class="sxs-lookup"><span data-stu-id="336ff-134">String</span></span>|<span data-ttu-id="336ff-135">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="336ff-135">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="336ff-136">url</span><span class="sxs-lookup"><span data-stu-id="336ff-136">url</span></span>|<span data-ttu-id="336ff-137">String</span><span class="sxs-lookup"><span data-stu-id="336ff-137">String</span></span>|<span data-ttu-id="336ff-138">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="336ff-138">Website url</span></span>|
|<span data-ttu-id="336ff-139">deviceCount</span><span class="sxs-lookup"><span data-stu-id="336ff-139">deviceCount</span></span>|<span data-ttu-id="336ff-140">Int32</span><span class="sxs-lookup"><span data-stu-id="336ff-140">Int32</span></span>|<span data-ttu-id="336ff-141">デバイス数</span><span class="sxs-lookup"><span data-stu-id="336ff-141">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="336ff-142">応答</span><span class="sxs-lookup"><span data-stu-id="336ff-142">Response</span></span>
<span data-ttu-id="336ff-143">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="336ff-143">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="336ff-144">例</span><span class="sxs-lookup"><span data-stu-id="336ff-144">Example</span></span>
### <a name="request"></a><span data-ttu-id="336ff-145">要求</span><span class="sxs-lookup"><span data-stu-id="336ff-145">Request</span></span>
<span data-ttu-id="336ff-146">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="336ff-146">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 48

{
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="336ff-147">応答</span><span class="sxs-lookup"><span data-stu-id="336ff-147">Response</span></span>
<span data-ttu-id="336ff-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="336ff-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





