---
title: windowsInformationProtectionNetworkLearningSummary の更新
description: windowsInformationProtectionNetworkLearningSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 30f5585149a1130a92c203394950c581655cc78b
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27329422"
---
# <a name="update-windowsinformationprotectionnetworklearningsummary"></a><span data-ttu-id="d4485-103">windowsInformationProtectionNetworkLearningSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d4485-103">Update windowsInformationProtectionNetworkLearningSummary</span></span>

> <span data-ttu-id="d4485-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="d4485-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="d4485-105">[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d4485-105">Update the properties of a [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="d4485-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="d4485-106">Prerequisites</span></span>
<span data-ttu-id="d4485-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d4485-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d4485-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d4485-109">Permission type</span></span>|<span data-ttu-id="d4485-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d4485-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d4485-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d4485-111">Delegated (work or school account)</span></span>|<span data-ttu-id="d4485-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d4485-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d4485-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d4485-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d4485-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4485-114">Not supported.</span></span>|
|<span data-ttu-id="d4485-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d4485-115">Application</span></span>|<span data-ttu-id="d4485-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d4485-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d4485-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d4485-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d4485-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4485-118">Request headers</span></span>
|<span data-ttu-id="d4485-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d4485-119">Header</span></span>|<span data-ttu-id="d4485-120">値</span><span class="sxs-lookup"><span data-stu-id="d4485-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d4485-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="d4485-121">Authorization</span></span>|<span data-ttu-id="d4485-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d4485-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d4485-123">Accept</span><span class="sxs-lookup"><span data-stu-id="d4485-123">Accept</span></span>|<span data-ttu-id="d4485-124">application/json</span><span class="sxs-lookup"><span data-stu-id="d4485-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d4485-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="d4485-125">Request body</span></span>
<span data-ttu-id="d4485-126">要求本文で、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d4485-126">In the request body, supply a JSON representation for the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object.</span></span>

<span data-ttu-id="d4485-127">次の表に、[windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d4485-127">The following table shows the properties that are required when you create the [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md).</span></span>

|<span data-ttu-id="d4485-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d4485-128">Property</span></span>|<span data-ttu-id="d4485-129">種類</span><span class="sxs-lookup"><span data-stu-id="d4485-129">Type</span></span>|<span data-ttu-id="d4485-130">説明</span><span class="sxs-lookup"><span data-stu-id="d4485-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d4485-131">ID</span><span class="sxs-lookup"><span data-stu-id="d4485-131">id</span></span>|<span data-ttu-id="d4485-132">String</span><span class="sxs-lookup"><span data-stu-id="d4485-132">String</span></span>|<span data-ttu-id="d4485-133">WindowsInformationProtectionNetworkLearningSummary の一意識別子。</span><span class="sxs-lookup"><span data-stu-id="d4485-133">Unique Identifier for the WindowsInformationProtectionNetworkLearningSummary.</span></span>|
|<span data-ttu-id="d4485-134">url</span><span class="sxs-lookup"><span data-stu-id="d4485-134">url</span></span>|<span data-ttu-id="d4485-135">String</span><span class="sxs-lookup"><span data-stu-id="d4485-135">String</span></span>|<span data-ttu-id="d4485-136">Web サイト URL</span><span class="sxs-lookup"><span data-stu-id="d4485-136">Website url</span></span>|
|<span data-ttu-id="d4485-137">deviceCount</span><span class="sxs-lookup"><span data-stu-id="d4485-137">deviceCount</span></span>|<span data-ttu-id="d4485-138">Int32</span><span class="sxs-lookup"><span data-stu-id="d4485-138">Int32</span></span>|<span data-ttu-id="d4485-139">デバイス数</span><span class="sxs-lookup"><span data-stu-id="d4485-139">Device Count</span></span>|



## <a name="response"></a><span data-ttu-id="d4485-140">応答</span><span class="sxs-lookup"><span data-stu-id="d4485-140">Response</span></span>
<span data-ttu-id="d4485-141">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d4485-141">If successful, this method returns a `200 OK` response code and an updated [windowsInformationProtectionNetworkLearningSummary](../resources/intune-wip-windowsinformationprotectionnetworklearningsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d4485-142">例</span><span class="sxs-lookup"><span data-stu-id="d4485-142">Example</span></span>
### <a name="request"></a><span data-ttu-id="d4485-143">要求</span><span class="sxs-lookup"><span data-stu-id="d4485-143">Request</span></span>
<span data-ttu-id="d4485-144">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d4485-144">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceManagement/windowsInformationProtectionNetworkLearningSummaries/{windowsInformationProtectionNetworkLearningSummaryId}
Content-type: application/json
Content-length: 137

{
  "@odata.type": "#microsoft.graph.windowsInformationProtectionNetworkLearningSummary",
  "url": "Url value",
  "deviceCount": 11
}
```

### <a name="response"></a><span data-ttu-id="d4485-145">応答</span><span class="sxs-lookup"><span data-stu-id="d4485-145">Response</span></span>
<span data-ttu-id="d4485-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d4485-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



