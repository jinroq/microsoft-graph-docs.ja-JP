---
title: userappinstallstatus の更新
description: userappinstallstatus オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: dce7bcd1e1c806c8f50aa6f4674104fd8d0e781b
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30966629"
---
# <a name="update-userappinstallstatus"></a><span data-ttu-id="ae130-103">userappinstallstatus の更新</span><span class="sxs-lookup"><span data-stu-id="ae130-103">Update userAppInstallStatus</span></span>

> <span data-ttu-id="ae130-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae130-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="ae130-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae130-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="ae130-106">[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="ae130-106">Update the properties of a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="ae130-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="ae130-107">Prerequisites</span></span>
<span data-ttu-id="ae130-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="ae130-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="ae130-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="ae130-110">Permission type</span></span>|<span data-ttu-id="ae130-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="ae130-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="ae130-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="ae130-112">Delegated (work or school account)</span></span>|<span data-ttu-id="ae130-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="ae130-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="ae130-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="ae130-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="ae130-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae130-115">Not supported.</span></span>|
|<span data-ttu-id="ae130-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="ae130-116">Application</span></span>|<span data-ttu-id="ae130-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="ae130-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="ae130-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="ae130-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses/{userAppInstallStatusId}
```

## <a name="request-headers"></a><span data-ttu-id="ae130-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae130-119">Request headers</span></span>
|<span data-ttu-id="ae130-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="ae130-120">Header</span></span>|<span data-ttu-id="ae130-121">値</span><span class="sxs-lookup"><span data-stu-id="ae130-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="ae130-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="ae130-122">Authorization</span></span>|<span data-ttu-id="ae130-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="ae130-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="ae130-124">承諾</span><span class="sxs-lookup"><span data-stu-id="ae130-124">Accept</span></span>|<span data-ttu-id="ae130-125">application/json</span><span class="sxs-lookup"><span data-stu-id="ae130-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="ae130-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="ae130-126">Request body</span></span>
<span data-ttu-id="ae130-127">要求本文で、 [userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="ae130-127">In the request body, supply a JSON representation for the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

<span data-ttu-id="ae130-128">次の表に、 [userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="ae130-128">The following table shows the properties that are required when you create the [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md).</span></span>

|<span data-ttu-id="ae130-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="ae130-129">Property</span></span>|<span data-ttu-id="ae130-130">型</span><span class="sxs-lookup"><span data-stu-id="ae130-130">Type</span></span>|<span data-ttu-id="ae130-131">説明</span><span class="sxs-lookup"><span data-stu-id="ae130-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="ae130-132">id</span><span class="sxs-lookup"><span data-stu-id="ae130-132">id</span></span>|<span data-ttu-id="ae130-133">String</span><span class="sxs-lookup"><span data-stu-id="ae130-133">String</span></span>|<span data-ttu-id="ae130-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="ae130-134">Key of the entity.</span></span>|
|<span data-ttu-id="ae130-135">userName</span><span class="sxs-lookup"><span data-stu-id="ae130-135">userName</span></span>|<span data-ttu-id="ae130-136">String</span><span class="sxs-lookup"><span data-stu-id="ae130-136">String</span></span>|<span data-ttu-id="ae130-137">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="ae130-137">User name.</span></span>|
|<span data-ttu-id="ae130-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="ae130-138">userPrincipalName</span></span>|<span data-ttu-id="ae130-139">String</span><span class="sxs-lookup"><span data-stu-id="ae130-139">String</span></span>|<span data-ttu-id="ae130-140">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="ae130-140">User Principal Name.</span></span>|
|<span data-ttu-id="ae130-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae130-141">installedDeviceCount</span></span>|<span data-ttu-id="ae130-142">Int32</span><span class="sxs-lookup"><span data-stu-id="ae130-142">Int32</span></span>|<span data-ttu-id="ae130-143">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae130-143">Installed Device Count.</span></span>|
|<span data-ttu-id="ae130-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae130-144">failedDeviceCount</span></span>|<span data-ttu-id="ae130-145">Int32</span><span class="sxs-lookup"><span data-stu-id="ae130-145">Int32</span></span>|<span data-ttu-id="ae130-146">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae130-146">Failed Device Count.</span></span>|
|<span data-ttu-id="ae130-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="ae130-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="ae130-148">Int32</span><span class="sxs-lookup"><span data-stu-id="ae130-148">Int32</span></span>|<span data-ttu-id="ae130-149">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="ae130-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="ae130-150">応答</span><span class="sxs-lookup"><span data-stu-id="ae130-150">Response</span></span>
<span data-ttu-id="ae130-151">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="ae130-151">If successful, this method returns a `200 OK` response code and an updated [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="ae130-152">例</span><span class="sxs-lookup"><span data-stu-id="ae130-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="ae130-153">要求</span><span class="sxs-lookup"><span data-stu-id="ae130-153">Request</span></span>
<span data-ttu-id="ae130-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="ae130-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="ae130-155">応答</span><span class="sxs-lookup"><span data-stu-id="ae130-155">Response</span></span>
<span data-ttu-id="ae130-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="ae130-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




