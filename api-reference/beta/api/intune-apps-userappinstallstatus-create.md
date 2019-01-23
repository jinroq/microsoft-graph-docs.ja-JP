---
title: UserAppInstallStatus を作成します。
description: 新しい userAppInstallStatus オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 3ebb03db9e8d9f0c2eab30ecebbee4dbf8832654
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29397870"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="70bd5-103">UserAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="70bd5-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="70bd5-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="70bd5-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="70bd5-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70bd5-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="70bd5-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70bd5-107">新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="70bd5-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70bd5-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="70bd5-108">Prerequisites</span></span>
<span data-ttu-id="70bd5-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70bd5-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="70bd5-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70bd5-111">Permission type</span></span>|<span data-ttu-id="70bd5-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="70bd5-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70bd5-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70bd5-113">Delegated (work or school account)</span></span>|<span data-ttu-id="70bd5-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70bd5-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70bd5-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70bd5-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70bd5-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70bd5-116">Not supported.</span></span>|
|<span data-ttu-id="70bd5-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70bd5-117">Application</span></span>|<span data-ttu-id="70bd5-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70bd5-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70bd5-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70bd5-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="70bd5-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70bd5-120">Request headers</span></span>
|<span data-ttu-id="70bd5-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70bd5-121">Header</span></span>|<span data-ttu-id="70bd5-122">値</span><span class="sxs-lookup"><span data-stu-id="70bd5-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70bd5-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="70bd5-123">Authorization</span></span>|<span data-ttu-id="70bd5-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="70bd5-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70bd5-125">Accept</span><span class="sxs-lookup"><span data-stu-id="70bd5-125">Accept</span></span>|<span data-ttu-id="70bd5-126">application/json</span><span class="sxs-lookup"><span data-stu-id="70bd5-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70bd5-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="70bd5-127">Request body</span></span>
<span data-ttu-id="70bd5-128">要求の本文に userAppInstallStatus オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="70bd5-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="70bd5-129">次の表は、userAppInstallStatus を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="70bd5-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="70bd5-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70bd5-130">Property</span></span>|<span data-ttu-id="70bd5-131">型</span><span class="sxs-lookup"><span data-stu-id="70bd5-131">Type</span></span>|<span data-ttu-id="70bd5-132">説明</span><span class="sxs-lookup"><span data-stu-id="70bd5-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70bd5-133">id</span><span class="sxs-lookup"><span data-stu-id="70bd5-133">id</span></span>|<span data-ttu-id="70bd5-134">String</span><span class="sxs-lookup"><span data-stu-id="70bd5-134">String</span></span>|<span data-ttu-id="70bd5-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="70bd5-135">Key of the entity.</span></span>|
|<span data-ttu-id="70bd5-136">userName</span><span class="sxs-lookup"><span data-stu-id="70bd5-136">userName</span></span>|<span data-ttu-id="70bd5-137">String</span><span class="sxs-lookup"><span data-stu-id="70bd5-137">String</span></span>|<span data-ttu-id="70bd5-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-138">User name.</span></span>|
|<span data-ttu-id="70bd5-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70bd5-139">userPrincipalName</span></span>|<span data-ttu-id="70bd5-140">String</span><span class="sxs-lookup"><span data-stu-id="70bd5-140">String</span></span>|<span data-ttu-id="70bd5-141">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-141">User Principal Name.</span></span>|
|<span data-ttu-id="70bd5-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bd5-142">installedDeviceCount</span></span>|<span data-ttu-id="70bd5-143">Int32</span><span class="sxs-lookup"><span data-stu-id="70bd5-143">Int32</span></span>|<span data-ttu-id="70bd5-144">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-144">Installed Device Count.</span></span>|
|<span data-ttu-id="70bd5-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bd5-145">failedDeviceCount</span></span>|<span data-ttu-id="70bd5-146">Int32</span><span class="sxs-lookup"><span data-stu-id="70bd5-146">Int32</span></span>|<span data-ttu-id="70bd5-147">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-147">Failed Device Count.</span></span>|
|<span data-ttu-id="70bd5-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70bd5-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="70bd5-149">Int32</span><span class="sxs-lookup"><span data-stu-id="70bd5-149">Int32</span></span>|<span data-ttu-id="70bd5-150">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="70bd5-151">応答</span><span class="sxs-lookup"><span data-stu-id="70bd5-151">Response</span></span>
<span data-ttu-id="70bd5-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="70bd5-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70bd5-153">例</span><span class="sxs-lookup"><span data-stu-id="70bd5-153">Example</span></span>

### <a name="request"></a><span data-ttu-id="70bd5-154">要求</span><span class="sxs-lookup"><span data-stu-id="70bd5-154">Request</span></span>
<span data-ttu-id="70bd5-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70bd5-155">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
Content-type: application/json
Content-length: 239

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="70bd5-156">応答</span><span class="sxs-lookup"><span data-stu-id="70bd5-156">Response</span></span>
<span data-ttu-id="70bd5-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="70bd5-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 288

{
  "@odata.type": "#microsoft.graph.userAppInstallStatus",
  "id": "14959a2a-9a2a-1495-2a9a-95142a9a9514",
  "userName": "User Name value",
  "userPrincipalName": "User Principal Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```




