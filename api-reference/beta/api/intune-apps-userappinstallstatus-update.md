---
title: UserAppInstallStatus の更新
description: UserAppInstallStatus オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 9f8cbcec45e1575c2bde8832c893c41a0eac0010
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934891"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="70058-103">UserAppInstallStatus の更新</span><span class="sxs-lookup"><span data-stu-id="70058-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="70058-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70058-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="70058-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="70058-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="70058-106">[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="70058-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="70058-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="70058-107">Prerequisites</span></span>
<span data-ttu-id="70058-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="70058-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="70058-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="70058-110">Permission type</span></span>|<span data-ttu-id="70058-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="70058-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="70058-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="70058-112">Delegated (work or school account)</span></span>|<span data-ttu-id="70058-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="70058-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="70058-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="70058-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="70058-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70058-115">Not supported.</span></span>|
|<span data-ttu-id="70058-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="70058-116">Application</span></span>|<span data-ttu-id="70058-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="70058-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="70058-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="70058-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="70058-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70058-119">Request headers</span></span>
|<span data-ttu-id="70058-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="70058-120">Header</span></span>|<span data-ttu-id="70058-121">値</span><span class="sxs-lookup"><span data-stu-id="70058-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="70058-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="70058-122">Authorization</span></span>|<span data-ttu-id="70058-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="70058-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="70058-124">承諾</span><span class="sxs-lookup"><span data-stu-id="70058-124">Accept</span></span>|<span data-ttu-id="70058-125">application/json</span><span class="sxs-lookup"><span data-stu-id="70058-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="70058-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="70058-126">Request body</span></span>
<span data-ttu-id="70058-127">要求本文で、 [Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="70058-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="70058-128">次の表に、 [Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="70058-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="70058-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="70058-129">Property</span></span>|<span data-ttu-id="70058-130">型</span><span class="sxs-lookup"><span data-stu-id="70058-130">Type</span></span>|<span data-ttu-id="70058-131">説明</span><span class="sxs-lookup"><span data-stu-id="70058-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="70058-132">id</span><span class="sxs-lookup"><span data-stu-id="70058-132">id</span></span>|<span data-ttu-id="70058-133">文字列</span><span class="sxs-lookup"><span data-stu-id="70058-133">String</span></span>|<span data-ttu-id="70058-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="70058-134">Key of the entity.</span></span>|
|<span data-ttu-id="70058-135">userName</span><span class="sxs-lookup"><span data-stu-id="70058-135">userName</span></span>|<span data-ttu-id="70058-136">String</span><span class="sxs-lookup"><span data-stu-id="70058-136">String</span></span>|<span data-ttu-id="70058-137">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="70058-137">User name.</span></span>|
|<span data-ttu-id="70058-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="70058-138">userPrincipalName</span></span>|<span data-ttu-id="70058-139">String</span><span class="sxs-lookup"><span data-stu-id="70058-139">String</span></span>|<span data-ttu-id="70058-140">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="70058-140">User Principal Name.</span></span>|
|<span data-ttu-id="70058-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70058-141">installedDeviceCount</span></span>|<span data-ttu-id="70058-142">Int32</span><span class="sxs-lookup"><span data-stu-id="70058-142">Int32</span></span>|<span data-ttu-id="70058-143">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70058-143">Installed Device Count.</span></span>|
|<span data-ttu-id="70058-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70058-144">failedDeviceCount</span></span>|<span data-ttu-id="70058-145">Int32</span><span class="sxs-lookup"><span data-stu-id="70058-145">Int32</span></span>|<span data-ttu-id="70058-146">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70058-146">Failed Device Count.</span></span>|
|<span data-ttu-id="70058-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="70058-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="70058-148">Int32</span><span class="sxs-lookup"><span data-stu-id="70058-148">Int32</span></span>|<span data-ttu-id="70058-149">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="70058-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="70058-150">応答</span><span class="sxs-lookup"><span data-stu-id="70058-150">Response</span></span>
<span data-ttu-id="70058-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="70058-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="70058-152">例</span><span class="sxs-lookup"><span data-stu-id="70058-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="70058-153">要求</span><span class="sxs-lookup"><span data-stu-id="70058-153">Request</span></span>
<span data-ttu-id="70058-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="70058-154">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
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

### <a name="response"></a><span data-ttu-id="70058-155">応答</span><span class="sxs-lookup"><span data-stu-id="70058-155">Response</span></span>
<span data-ttu-id="70058-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="70058-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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




