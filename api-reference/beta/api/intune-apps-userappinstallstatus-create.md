---
title: UserAppInstallStatus の作成
description: 新しい userAppInstallStatus オブジェクトを作成します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: 8cf9a460bb6188fe7875d962db27f2788189ede6
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328943"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="37abe-103">UserAppInstallStatus の作成</span><span class="sxs-lookup"><span data-stu-id="37abe-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="37abe-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37abe-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="37abe-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="37abe-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="37abe-106">新しい[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="37abe-106">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="37abe-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="37abe-107">Prerequisites</span></span>
<span data-ttu-id="37abe-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="37abe-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="37abe-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="37abe-110">Permission type</span></span>|<span data-ttu-id="37abe-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="37abe-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="37abe-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="37abe-112">Delegated (work or school account)</span></span>|<span data-ttu-id="37abe-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37abe-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="37abe-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="37abe-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="37abe-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="37abe-115">Not supported.</span></span>|
|<span data-ttu-id="37abe-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="37abe-116">Application</span></span>|<span data-ttu-id="37abe-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="37abe-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="37abe-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="37abe-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="37abe-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37abe-119">Request headers</span></span>
|<span data-ttu-id="37abe-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="37abe-120">Header</span></span>|<span data-ttu-id="37abe-121">値</span><span class="sxs-lookup"><span data-stu-id="37abe-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="37abe-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="37abe-122">Authorization</span></span>|<span data-ttu-id="37abe-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="37abe-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="37abe-124">承諾</span><span class="sxs-lookup"><span data-stu-id="37abe-124">Accept</span></span>|<span data-ttu-id="37abe-125">application/json</span><span class="sxs-lookup"><span data-stu-id="37abe-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="37abe-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="37abe-126">Request body</span></span>
<span data-ttu-id="37abe-127">要求本文で、userAppInstallStatus オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="37abe-127">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="37abe-128">次の表に、userAppInstallStatus の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="37abe-128">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="37abe-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="37abe-129">Property</span></span>|<span data-ttu-id="37abe-130">型</span><span class="sxs-lookup"><span data-stu-id="37abe-130">Type</span></span>|<span data-ttu-id="37abe-131">説明</span><span class="sxs-lookup"><span data-stu-id="37abe-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="37abe-132">id</span><span class="sxs-lookup"><span data-stu-id="37abe-132">id</span></span>|<span data-ttu-id="37abe-133">文字列</span><span class="sxs-lookup"><span data-stu-id="37abe-133">String</span></span>|<span data-ttu-id="37abe-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="37abe-134">Key of the entity.</span></span>|
|<span data-ttu-id="37abe-135">userName</span><span class="sxs-lookup"><span data-stu-id="37abe-135">userName</span></span>|<span data-ttu-id="37abe-136">String</span><span class="sxs-lookup"><span data-stu-id="37abe-136">String</span></span>|<span data-ttu-id="37abe-137">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="37abe-137">User name.</span></span>|
|<span data-ttu-id="37abe-138">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="37abe-138">userPrincipalName</span></span>|<span data-ttu-id="37abe-139">String</span><span class="sxs-lookup"><span data-stu-id="37abe-139">String</span></span>|<span data-ttu-id="37abe-140">ユーザープリンシパル名。</span><span class="sxs-lookup"><span data-stu-id="37abe-140">User Principal Name.</span></span>|
|<span data-ttu-id="37abe-141">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37abe-141">installedDeviceCount</span></span>|<span data-ttu-id="37abe-142">Int32</span><span class="sxs-lookup"><span data-stu-id="37abe-142">Int32</span></span>|<span data-ttu-id="37abe-143">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="37abe-143">Installed Device Count.</span></span>|
|<span data-ttu-id="37abe-144">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37abe-144">failedDeviceCount</span></span>|<span data-ttu-id="37abe-145">Int32</span><span class="sxs-lookup"><span data-stu-id="37abe-145">Int32</span></span>|<span data-ttu-id="37abe-146">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="37abe-146">Failed Device Count.</span></span>|
|<span data-ttu-id="37abe-147">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="37abe-147">notInstalledDeviceCount</span></span>|<span data-ttu-id="37abe-148">Int32</span><span class="sxs-lookup"><span data-stu-id="37abe-148">Int32</span></span>|<span data-ttu-id="37abe-149">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="37abe-149">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="37abe-150">応答</span><span class="sxs-lookup"><span data-stu-id="37abe-150">Response</span></span>
<span data-ttu-id="37abe-151">成功した場合、このメソッド`201 Created`は応答コードと、応答本文で[Userappinstallstatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="37abe-151">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="37abe-152">例</span><span class="sxs-lookup"><span data-stu-id="37abe-152">Example</span></span>

### <a name="request"></a><span data-ttu-id="37abe-153">要求</span><span class="sxs-lookup"><span data-stu-id="37abe-153">Request</span></span>
<span data-ttu-id="37abe-154">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="37abe-154">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="37abe-155">応答</span><span class="sxs-lookup"><span data-stu-id="37abe-155">Response</span></span>
<span data-ttu-id="37abe-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="37abe-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






