---
title: WindowsManagementAppHealthSummary を更新します。
description: WindowsManagementAppHealthSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: d7e8c077b8f06b9647e34a18fd5aa92987272e77
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29394167"
---
# <a name="update-windowsmanagementapphealthsummary"></a><span data-ttu-id="14281-103">WindowsManagementAppHealthSummary を更新します。</span><span class="sxs-lookup"><span data-stu-id="14281-103">Update windowsManagementAppHealthSummary</span></span>

> <span data-ttu-id="14281-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="14281-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="14281-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14281-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="14281-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="14281-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="14281-107">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="14281-107">Update the properties of a [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="14281-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="14281-108">Prerequisites</span></span>
<span data-ttu-id="14281-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="14281-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="14281-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="14281-111">Permission type</span></span>|<span data-ttu-id="14281-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="14281-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="14281-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="14281-113">Delegated (work or school account)</span></span>|<span data-ttu-id="14281-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="14281-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="14281-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="14281-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="14281-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14281-116">Not supported.</span></span>|
|<span data-ttu-id="14281-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="14281-117">Application</span></span>|<span data-ttu-id="14281-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="14281-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="14281-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="14281-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp/healthSummary
```

## <a name="request-headers"></a><span data-ttu-id="14281-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14281-120">Request headers</span></span>
|<span data-ttu-id="14281-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="14281-121">Header</span></span>|<span data-ttu-id="14281-122">値</span><span class="sxs-lookup"><span data-stu-id="14281-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="14281-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="14281-123">Authorization</span></span>|<span data-ttu-id="14281-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="14281-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="14281-125">Accept</span><span class="sxs-lookup"><span data-stu-id="14281-125">Accept</span></span>|<span data-ttu-id="14281-126">application/json</span><span class="sxs-lookup"><span data-stu-id="14281-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="14281-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="14281-127">Request body</span></span>
<span data-ttu-id="14281-128">要求の本文に[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="14281-128">In the request body, supply a JSON representation for the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object.</span></span>

<span data-ttu-id="14281-129">[WindowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="14281-129">The following table shows the properties that are required when you create the [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md).</span></span>

|<span data-ttu-id="14281-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="14281-130">Property</span></span>|<span data-ttu-id="14281-131">型</span><span class="sxs-lookup"><span data-stu-id="14281-131">Type</span></span>|<span data-ttu-id="14281-132">説明</span><span class="sxs-lookup"><span data-stu-id="14281-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="14281-133">id</span><span class="sxs-lookup"><span data-stu-id="14281-133">id</span></span>|<span data-ttu-id="14281-134">String</span><span class="sxs-lookup"><span data-stu-id="14281-134">String</span></span>|<span data-ttu-id="14281-135">Windows 管理アプリケーションの稼働状態の概要エンティティのキーです。</span><span class="sxs-lookup"><span data-stu-id="14281-135">Key of the Windows management app health summary entity.</span></span>|
|<span data-ttu-id="14281-136">healthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14281-136">healthyDeviceCount</span></span>|<span data-ttu-id="14281-137">Int32</span><span class="sxs-lookup"><span data-stu-id="14281-137">Int32</span></span>|<span data-ttu-id="14281-138">正常なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="14281-138">Healthy device count.</span></span>|
|<span data-ttu-id="14281-139">unhealthyDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14281-139">unhealthyDeviceCount</span></span>|<span data-ttu-id="14281-140">Int32</span><span class="sxs-lookup"><span data-stu-id="14281-140">Int32</span></span>|<span data-ttu-id="14281-141">問題のあるデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="14281-141">Unhealthy device count.</span></span>|
|<span data-ttu-id="14281-142">unknownDeviceCount</span><span class="sxs-lookup"><span data-stu-id="14281-142">unknownDeviceCount</span></span>|<span data-ttu-id="14281-143">Int32</span><span class="sxs-lookup"><span data-stu-id="14281-143">Int32</span></span>|<span data-ttu-id="14281-144">不明なデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="14281-144">Unknown device count.</span></span>|



## <a name="response"></a><span data-ttu-id="14281-145">応答</span><span class="sxs-lookup"><span data-stu-id="14281-145">Response</span></span>
<span data-ttu-id="14281-146">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="14281-146">If successful, this method returns a `200 OK` response code and an updated [windowsManagementAppHealthSummary](../resources/intune-devices-windowsmanagementapphealthsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="14281-147">例</span><span class="sxs-lookup"><span data-stu-id="14281-147">Example</span></span>

### <a name="request"></a><span data-ttu-id="14281-148">要求</span><span class="sxs-lookup"><span data-stu-id="14281-148">Request</span></span>
<span data-ttu-id="14281-149">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="14281-149">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp/healthSummary
Content-type: application/json
Content-length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementAppHealthSummary",
  "healthyDeviceCount": 2,
  "unhealthyDeviceCount": 4,
  "unknownDeviceCount": 2
}
```

### <a name="response"></a><span data-ttu-id="14281-150">応答</span><span class="sxs-lookup"><span data-stu-id="14281-150">Response</span></span>
<span data-ttu-id="14281-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="14281-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




