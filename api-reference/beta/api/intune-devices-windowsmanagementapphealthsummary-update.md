---
title: WindowsManagementAppHealthSummary を更新します。
description: WindowsManagementAppHealthSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 274ffcc65706f7d730815d4a8350af2dee68f763
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27307071"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="f2dd4-103">WindowsManagementAppHealthSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="f2dd4-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f2dd4-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f2dd4-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f2dd4-107">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f2dd4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f2dd4-108">Prerequisites</span></span>
<span data-ttu-id="f2dd4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f2dd4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f2dd4-111">Permission type</span></span>|<span data-ttu-id="f2dd4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f2dd4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f2dd4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f2dd4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f2dd4-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f2dd4-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f2dd4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f2dd4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f2dd4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-116">Not supported.</span></span>|
|<span data-ttu-id="f2dd4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f2dd4-117">Application</span></span>|<span data-ttu-id="f2dd4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f2dd4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f2dd4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="f2dd4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2dd4-120">Request headers</span></span>
|<span data-ttu-id="f2dd4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f2dd4-121">Header</span></span>|<span data-ttu-id="f2dd4-122">値</span><span class="sxs-lookup"><span data-stu-id="f2dd4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f2dd4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f2dd4-123">Authorization</span></span>|<span data-ttu-id="f2dd4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f2dd4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f2dd4-125">Accept</span></span>|<span data-ttu-id="f2dd4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f2dd4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f2dd4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f2dd4-127">Request body</span></span>
<span data-ttu-id="f2dd4-128">要求の本文に[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="f2dd4-129">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="f2dd4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f2dd4-130">Property</span></span>|<span data-ttu-id="f2dd4-131">種類</span><span class="sxs-lookup"><span data-stu-id="f2dd4-131">Type</span></span>|<span data-ttu-id="f2dd4-132">説明</span><span class="sxs-lookup"><span data-stu-id="f2dd4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f2dd4-133">ID</span><span class="sxs-lookup"><span data-stu-id="f2dd4-133">id</span></span>|<span data-ttu-id="f2dd4-134">String</span><span class="sxs-lookup"><span data-stu-id="f2dd4-134">String</span></span>|<span data-ttu-id="f2dd4-135">Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="f2dd4-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2dd4-136">healthyDeviceCount</span></span>|<span data-ttu-id="f2dd4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="f2dd4-137">Int32</span></span>|<span data-ttu-id="f2dd4-138">正常なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-138">Healthy device count.</span></span>|
|<span data-ttu-id="f2dd4-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2dd4-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="f2dd4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="f2dd4-140">Int32</span></span>|<span data-ttu-id="f2dd4-141">問題のあるデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="f2dd4-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f2dd4-142">unknownDeviceCount</span></span>|<span data-ttu-id="f2dd4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f2dd4-143">Int32</span></span>|<span data-ttu-id="f2dd4-144">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f2dd4-145">応答</span><span class="sxs-lookup"><span data-stu-id="f2dd4-145">Response</span></span>
<span data-ttu-id="f2dd4-146">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f2dd4-147">例</span><span class="sxs-lookup"><span data-stu-id="f2dd4-147">Example</span></span>
### <a name="request"></a><span data-ttu-id="f2dd4-148">要求</span><span class="sxs-lookup"><span data-stu-id="f2dd4-148">Request</span></span>
<span data-ttu-id="f2dd4-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 89

{
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="f2dd4-150">応答</span><span class="sxs-lookup"><span data-stu-id="f2dd4-150">Response</span></span>
<span data-ttu-id="f2dd4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f2dd4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 210

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "id": "a9d38a9e-8a9e-a9d3-9e8a-d3a99e8ad3a9",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```





