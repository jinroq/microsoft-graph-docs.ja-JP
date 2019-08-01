---
title: eBookInstallSummary の更新
description: eBookInstallSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: b8b57abc37de65d4040ae4f02bb825111ecefca4
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "36013564"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="51d57-103">eBookInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="51d57-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="51d57-104">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="51d57-104">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="51d57-105">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="51d57-105">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="51d57-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="51d57-106">Prerequisites</span></span>
<span data-ttu-id="51d57-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="51d57-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="51d57-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="51d57-109">Permission type</span></span>|<span data-ttu-id="51d57-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="51d57-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="51d57-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="51d57-111">Delegated (work or school account)</span></span>|<span data-ttu-id="51d57-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="51d57-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="51d57-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="51d57-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="51d57-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51d57-114">Not supported.</span></span>|
|<span data-ttu-id="51d57-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="51d57-115">Application</span></span>|<span data-ttu-id="51d57-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="51d57-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="51d57-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="51d57-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="51d57-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51d57-118">Request headers</span></span>
|<span data-ttu-id="51d57-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="51d57-119">Header</span></span>|<span data-ttu-id="51d57-120">値</span><span class="sxs-lookup"><span data-stu-id="51d57-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="51d57-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="51d57-121">Authorization</span></span>|<span data-ttu-id="51d57-122">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="51d57-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="51d57-123">承諾</span><span class="sxs-lookup"><span data-stu-id="51d57-123">Accept</span></span>|<span data-ttu-id="51d57-124">application/json</span><span class="sxs-lookup"><span data-stu-id="51d57-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="51d57-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="51d57-125">Request body</span></span>
<span data-ttu-id="51d57-126">要求本文で、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="51d57-126">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="51d57-127">次の表に、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="51d57-127">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="51d57-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="51d57-128">Property</span></span>|<span data-ttu-id="51d57-129">型</span><span class="sxs-lookup"><span data-stu-id="51d57-129">Type</span></span>|<span data-ttu-id="51d57-130">説明</span><span class="sxs-lookup"><span data-stu-id="51d57-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="51d57-131">id</span><span class="sxs-lookup"><span data-stu-id="51d57-131">id</span></span>|<span data-ttu-id="51d57-132">String</span><span class="sxs-lookup"><span data-stu-id="51d57-132">String</span></span>|<span data-ttu-id="51d57-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="51d57-133">Key of the entity.</span></span>|
|<span data-ttu-id="51d57-134">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51d57-134">installedDeviceCount</span></span>|<span data-ttu-id="51d57-135">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-135">Int32</span></span>|<span data-ttu-id="51d57-136">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-136">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="51d57-137">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51d57-137">failedDeviceCount</span></span>|<span data-ttu-id="51d57-138">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-138">Int32</span></span>|<span data-ttu-id="51d57-139">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-139">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="51d57-140">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="51d57-140">notInstalledDeviceCount</span></span>|<span data-ttu-id="51d57-141">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-141">Int32</span></span>|<span data-ttu-id="51d57-142">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-142">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="51d57-143">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="51d57-143">installedUserCount</span></span>|<span data-ttu-id="51d57-144">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-144">Int32</span></span>|<span data-ttu-id="51d57-145">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-145">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="51d57-146">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="51d57-146">failedUserCount</span></span>|<span data-ttu-id="51d57-147">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-147">Int32</span></span>|<span data-ttu-id="51d57-148">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-148">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="51d57-149">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="51d57-149">notInstalledUserCount</span></span>|<span data-ttu-id="51d57-150">Int32</span><span class="sxs-lookup"><span data-stu-id="51d57-150">Int32</span></span>|<span data-ttu-id="51d57-151">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="51d57-151">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="51d57-152">応答</span><span class="sxs-lookup"><span data-stu-id="51d57-152">Response</span></span>
<span data-ttu-id="51d57-153">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="51d57-153">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="51d57-154">例</span><span class="sxs-lookup"><span data-stu-id="51d57-154">Example</span></span>

### <a name="request"></a><span data-ttu-id="51d57-155">要求</span><span class="sxs-lookup"><span data-stu-id="51d57-155">Request</span></span>
<span data-ttu-id="51d57-156">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="51d57-156">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
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

### <a name="response"></a><span data-ttu-id="51d57-157">応答</span><span class="sxs-lookup"><span data-stu-id="51d57-157">Response</span></span>
<span data-ttu-id="51d57-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="51d57-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



