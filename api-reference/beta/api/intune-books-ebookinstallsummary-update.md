---
title: eBookInstallSummary の更新
description: eBookInstallSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 85e94a16799b9ee56c28041549b1d21692013599
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29421166"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="ae4d4-103">eBookInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="ae4d4-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="ae4d4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="ae4d4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="ae4d4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae4d4-107">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae4d4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae4d4-108">Prerequisites</span></span>
<span data-ttu-id="ae4d4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="ae4d4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae4d4-111">Permission type</span></span>|<span data-ttu-id="ae4d4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae4d4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae4d4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae4d4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="ae4d4-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae4d4-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae4d4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae4d4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae4d4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-116">Not supported.</span></span>|
|<span data-ttu-id="ae4d4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae4d4-117">Application</span></span>|<span data-ttu-id="ae4d4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae4d4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae4d4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="ae4d4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae4d4-120">Request headers</span></span>
|<span data-ttu-id="ae4d4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae4d4-121">Header</span></span>|<span data-ttu-id="ae4d4-122">値</span><span class="sxs-lookup"><span data-stu-id="ae4d4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae4d4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae4d4-123">Authorization</span></span>|<span data-ttu-id="ae4d4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae4d4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="ae4d4-125">Accept</span></span>|<span data-ttu-id="ae4d4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="ae4d4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae4d4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae4d4-127">Request body</span></span>
<span data-ttu-id="ae4d4-128">要求本文で、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="ae4d4-129">次の表に、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="ae4d4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae4d4-130">Property</span></span>|<span data-ttu-id="ae4d4-131">型</span><span class="sxs-lookup"><span data-stu-id="ae4d4-131">Type</span></span>|<span data-ttu-id="ae4d4-132">説明</span><span class="sxs-lookup"><span data-stu-id="ae4d4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae4d4-133">id</span><span class="sxs-lookup"><span data-stu-id="ae4d4-133">id</span></span>|<span data-ttu-id="ae4d4-134">String</span><span class="sxs-lookup"><span data-stu-id="ae4d4-134">String</span></span>|<span data-ttu-id="ae4d4-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-135">Key of the entity.</span></span>|
|<span data-ttu-id="ae4d4-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-136">installedDeviceCount</span></span>|<span data-ttu-id="ae4d4-137">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-137">Int32</span></span>|<span data-ttu-id="ae4d4-138">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="ae4d4-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-139">failedDeviceCount</span></span>|<span data-ttu-id="ae4d4-140">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-140">Int32</span></span>|<span data-ttu-id="ae4d4-141">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="ae4d4-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="ae4d4-143">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-143">Int32</span></span>|<span data-ttu-id="ae4d4-144">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="ae4d4-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-145">installedUserCount</span></span>|<span data-ttu-id="ae4d4-146">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-146">Int32</span></span>|<span data-ttu-id="ae4d4-147">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="ae4d4-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-148">failedUserCount</span></span>|<span data-ttu-id="ae4d4-149">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-149">Int32</span></span>|<span data-ttu-id="ae4d4-150">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="ae4d4-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="ae4d4-151">notInstalledUserCount</span></span>|<span data-ttu-id="ae4d4-152">Int32</span><span class="sxs-lookup"><span data-stu-id="ae4d4-152">Int32</span></span>|<span data-ttu-id="ae4d4-153">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="ae4d4-154">応答</span><span class="sxs-lookup"><span data-stu-id="ae4d4-154">Response</span></span>
<span data-ttu-id="ae4d4-155">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae4d4-156">例</span><span class="sxs-lookup"><span data-stu-id="ae4d4-156">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae4d4-157">要求</span><span class="sxs-lookup"><span data-stu-id="ae4d4-157">Request</span></span>
<span data-ttu-id="ae4d4-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 236

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="ae4d4-159">応答</span><span class="sxs-lookup"><span data-stu-id="ae4d4-159">Response</span></span>
<span data-ttu-id="ae4d4-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae4d4-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 285

{
  "@odata.type": "#microsoft.graph.eBookInstallSummary",
  "id": "9708ad78-ad78-9708-78ad-089778ad0897",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```




