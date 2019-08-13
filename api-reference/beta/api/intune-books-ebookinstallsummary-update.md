---
title: eBookInstallSummary の更新
description: eBookInstallSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 1b61b0b0ca33ca6314cb9f9e4b9672a5493c1747
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36336069"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="8fcab-103">eBookInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="8fcab-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="8fcab-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fcab-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="8fcab-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fcab-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="8fcab-106">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="8fcab-106">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="8fcab-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="8fcab-107">Prerequisites</span></span>
<span data-ttu-id="8fcab-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="8fcab-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="8fcab-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="8fcab-110">Permission type</span></span>|<span data-ttu-id="8fcab-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="8fcab-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="8fcab-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="8fcab-112">Delegated (work or school account)</span></span>|<span data-ttu-id="8fcab-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fcab-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="8fcab-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="8fcab-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="8fcab-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="8fcab-115">Not supported.</span></span>|
|<span data-ttu-id="8fcab-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="8fcab-116">Application</span></span>|<span data-ttu-id="8fcab-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="8fcab-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="8fcab-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="8fcab-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="8fcab-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fcab-119">Request headers</span></span>
|<span data-ttu-id="8fcab-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="8fcab-120">Header</span></span>|<span data-ttu-id="8fcab-121">値</span><span class="sxs-lookup"><span data-stu-id="8fcab-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="8fcab-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="8fcab-122">Authorization</span></span>|<span data-ttu-id="8fcab-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="8fcab-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="8fcab-124">承諾</span><span class="sxs-lookup"><span data-stu-id="8fcab-124">Accept</span></span>|<span data-ttu-id="8fcab-125">application/json</span><span class="sxs-lookup"><span data-stu-id="8fcab-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="8fcab-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="8fcab-126">Request body</span></span>
<span data-ttu-id="8fcab-127">要求本文で、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="8fcab-127">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="8fcab-128">次の表に、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="8fcab-128">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="8fcab-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="8fcab-129">Property</span></span>|<span data-ttu-id="8fcab-130">型</span><span class="sxs-lookup"><span data-stu-id="8fcab-130">Type</span></span>|<span data-ttu-id="8fcab-131">説明</span><span class="sxs-lookup"><span data-stu-id="8fcab-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="8fcab-132">id</span><span class="sxs-lookup"><span data-stu-id="8fcab-132">id</span></span>|<span data-ttu-id="8fcab-133">String</span><span class="sxs-lookup"><span data-stu-id="8fcab-133">String</span></span>|<span data-ttu-id="8fcab-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="8fcab-134">Key of the entity.</span></span>|
|<span data-ttu-id="8fcab-135">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-135">installedDeviceCount</span></span>|<span data-ttu-id="8fcab-136">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-136">Int32</span></span>|<span data-ttu-id="8fcab-137">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-137">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="8fcab-138">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-138">failedDeviceCount</span></span>|<span data-ttu-id="8fcab-139">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-139">Int32</span></span>|<span data-ttu-id="8fcab-140">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-140">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="8fcab-141">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-141">notInstalledDeviceCount</span></span>|<span data-ttu-id="8fcab-142">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-142">Int32</span></span>|<span data-ttu-id="8fcab-143">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-143">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="8fcab-144">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-144">installedUserCount</span></span>|<span data-ttu-id="8fcab-145">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-145">Int32</span></span>|<span data-ttu-id="8fcab-146">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-146">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="8fcab-147">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-147">failedUserCount</span></span>|<span data-ttu-id="8fcab-148">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-148">Int32</span></span>|<span data-ttu-id="8fcab-149">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-149">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="8fcab-150">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="8fcab-150">notInstalledUserCount</span></span>|<span data-ttu-id="8fcab-151">Int32</span><span class="sxs-lookup"><span data-stu-id="8fcab-151">Int32</span></span>|<span data-ttu-id="8fcab-152">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="8fcab-152">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="8fcab-153">応答</span><span class="sxs-lookup"><span data-stu-id="8fcab-153">Response</span></span>
<span data-ttu-id="8fcab-154">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="8fcab-154">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="8fcab-155">例</span><span class="sxs-lookup"><span data-stu-id="8fcab-155">Example</span></span>

### <a name="request"></a><span data-ttu-id="8fcab-156">要求</span><span class="sxs-lookup"><span data-stu-id="8fcab-156">Request</span></span>
<span data-ttu-id="8fcab-157">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="8fcab-157">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="8fcab-158">応答</span><span class="sxs-lookup"><span data-stu-id="8fcab-158">Response</span></span>
<span data-ttu-id="8fcab-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="8fcab-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






