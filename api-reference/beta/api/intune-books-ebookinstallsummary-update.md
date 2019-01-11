---
title: eBookInstallSummary の更新
description: eBookInstallSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.openlocfilehash: d877e2c0af7df6c0d5c8743c1d43fd8c7d6298a6
ms.sourcegitcommit: d2b3ca32602ffa76cc7925d7f4d1e2258e611ea5
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/11/2019
ms.locfileid: "27874635"
---
# <a name="update-ebookinstallsummary"></a><span data-ttu-id="22b48-103">eBookInstallSummary の更新</span><span class="sxs-lookup"><span data-stu-id="22b48-103">Update eBookInstallSummary</span></span>

> <span data-ttu-id="22b48-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="22b48-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="22b48-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22b48-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="22b48-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="22b48-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="22b48-107">[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="22b48-107">Update the properties of a [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="22b48-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="22b48-108">Prerequisites</span></span>
<span data-ttu-id="22b48-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="22b48-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="22b48-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="22b48-111">Permission type</span></span>|<span data-ttu-id="22b48-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="22b48-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="22b48-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="22b48-113">Delegated (work or school account)</span></span>|<span data-ttu-id="22b48-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="22b48-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="22b48-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="22b48-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="22b48-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22b48-116">Not supported.</span></span>|
|<span data-ttu-id="22b48-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="22b48-117">Application</span></span>|<span data-ttu-id="22b48-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="22b48-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="22b48-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="22b48-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
```

## <a name="request-headers"></a><span data-ttu-id="22b48-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22b48-120">Request headers</span></span>
|<span data-ttu-id="22b48-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="22b48-121">Header</span></span>|<span data-ttu-id="22b48-122">値</span><span class="sxs-lookup"><span data-stu-id="22b48-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="22b48-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="22b48-123">Authorization</span></span>|<span data-ttu-id="22b48-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="22b48-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="22b48-125">Accept</span><span class="sxs-lookup"><span data-stu-id="22b48-125">Accept</span></span>|<span data-ttu-id="22b48-126">application/json</span><span class="sxs-lookup"><span data-stu-id="22b48-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="22b48-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="22b48-127">Request body</span></span>
<span data-ttu-id="22b48-128">要求本文で、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="22b48-128">In the request body, supply a JSON representation for the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object.</span></span>

<span data-ttu-id="22b48-129">次の表に、[eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="22b48-129">The following table shows the properties that are required when you create the [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md).</span></span>

|<span data-ttu-id="22b48-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="22b48-130">Property</span></span>|<span data-ttu-id="22b48-131">種類</span><span class="sxs-lookup"><span data-stu-id="22b48-131">Type</span></span>|<span data-ttu-id="22b48-132">説明</span><span class="sxs-lookup"><span data-stu-id="22b48-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="22b48-133">ID</span><span class="sxs-lookup"><span data-stu-id="22b48-133">id</span></span>|<span data-ttu-id="22b48-134">String</span><span class="sxs-lookup"><span data-stu-id="22b48-134">String</span></span>|<span data-ttu-id="22b48-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="22b48-135">Key of the entity.</span></span>|
|<span data-ttu-id="22b48-136">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22b48-136">installedDeviceCount</span></span>|<span data-ttu-id="22b48-137">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-137">Int32</span></span>|<span data-ttu-id="22b48-138">このブックが正常にインストールされたデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-138">Number of Devices that have successfully installed this book.</span></span>|
|<span data-ttu-id="22b48-139">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22b48-139">failedDeviceCount</span></span>|<span data-ttu-id="22b48-140">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-140">Int32</span></span>|<span data-ttu-id="22b48-141">このブックのインストールが失敗したデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-141">Number of Devices that have failed to install this book.</span></span>|
|<span data-ttu-id="22b48-142">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="22b48-142">notInstalledDeviceCount</span></span>|<span data-ttu-id="22b48-143">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-143">Int32</span></span>|<span data-ttu-id="22b48-144">このブックがインストールされていないデバイスの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-144">Number of Devices that does not have this book installed.</span></span>|
|<span data-ttu-id="22b48-145">installedUserCount</span><span class="sxs-lookup"><span data-stu-id="22b48-145">installedUserCount</span></span>|<span data-ttu-id="22b48-146">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-146">Int32</span></span>|<span data-ttu-id="22b48-147">このブックがすべて正常にインストールされたデバイスを所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-147">Number of Users whose devices have all succeeded to install this book.</span></span>|
|<span data-ttu-id="22b48-148">failedUserCount</span><span class="sxs-lookup"><span data-stu-id="22b48-148">failedUserCount</span></span>|<span data-ttu-id="22b48-149">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-149">Int32</span></span>|<span data-ttu-id="22b48-150">このブックのインストールが失敗したデバイスを 1 台以上所有しているユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-150">Number of Users that have 1 or more device that failed to install this book.</span></span>|
|<span data-ttu-id="22b48-151">notInstalledUserCount</span><span class="sxs-lookup"><span data-stu-id="22b48-151">notInstalledUserCount</span></span>|<span data-ttu-id="22b48-152">Int32</span><span class="sxs-lookup"><span data-stu-id="22b48-152">Int32</span></span>|<span data-ttu-id="22b48-153">このブックをインストールしていないユーザーの数。</span><span class="sxs-lookup"><span data-stu-id="22b48-153">Number of Users that did not install this book.</span></span>|



## <a name="response"></a><span data-ttu-id="22b48-154">応答</span><span class="sxs-lookup"><span data-stu-id="22b48-154">Response</span></span>
<span data-ttu-id="22b48-155">成功した場合、このメソッドは `200 OK` 応答コードと、更新された [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) オブジェクトを応答本文で返します。</span><span class="sxs-lookup"><span data-stu-id="22b48-155">If successful, this method returns a `200 OK` response code and an updated [eBookInstallSummary](../resources/intune-books-ebookinstallsummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="22b48-156">例</span><span class="sxs-lookup"><span data-stu-id="22b48-156">Example</span></span>
### <a name="request"></a><span data-ttu-id="22b48-157">要求</span><span class="sxs-lookup"><span data-stu-id="22b48-157">Request</span></span>
<span data-ttu-id="22b48-158">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="22b48-158">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/installSummary
Content-type: application/json
Content-length: 178

{
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7,
  "installedUserCount": 2,
  "failedUserCount": 15,
  "notInstalledUserCount": 5
}
```

### <a name="response"></a><span data-ttu-id="22b48-159">応答</span><span class="sxs-lookup"><span data-stu-id="22b48-159">Response</span></span>
<span data-ttu-id="22b48-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="22b48-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





