---
title: UserAppInstallStatus を作成します。
description: 新しい userAppInstallStatus オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: ac22969b04f2c9191e521a3df8a51bc2d0cc3343
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27985229"
---
# <a name="create-userappinstallstatus"></a><span data-ttu-id="f542e-103">UserAppInstallStatus を作成します。</span><span class="sxs-lookup"><span data-stu-id="f542e-103">Create userAppInstallStatus</span></span>

> <span data-ttu-id="f542e-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="f542e-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="f542e-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f542e-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="f542e-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="f542e-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="f542e-107">新しい[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="f542e-107">Create a new [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="f542e-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="f542e-108">Prerequisites</span></span>
<span data-ttu-id="f542e-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f542e-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f542e-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f542e-111">Permission type</span></span>|<span data-ttu-id="f542e-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f542e-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f542e-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f542e-113">Delegated (work or school account)</span></span>|<span data-ttu-id="f542e-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f542e-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f542e-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f542e-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f542e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f542e-116">Not supported.</span></span>|
|<span data-ttu-id="f542e-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f542e-117">Application</span></span>|<span data-ttu-id="f542e-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f542e-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f542e-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f542e-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/mobileApps/{mobileAppId}/userStatuses
```

## <a name="request-headers"></a><span data-ttu-id="f542e-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f542e-120">Request headers</span></span>
|<span data-ttu-id="f542e-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f542e-121">Header</span></span>|<span data-ttu-id="f542e-122">値</span><span class="sxs-lookup"><span data-stu-id="f542e-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f542e-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="f542e-123">Authorization</span></span>|<span data-ttu-id="f542e-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="f542e-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f542e-125">Accept</span><span class="sxs-lookup"><span data-stu-id="f542e-125">Accept</span></span>|<span data-ttu-id="f542e-126">application/json</span><span class="sxs-lookup"><span data-stu-id="f542e-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f542e-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="f542e-127">Request body</span></span>
<span data-ttu-id="f542e-128">要求の本文に userAppInstallStatus オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="f542e-128">In the request body, supply a JSON representation for the userAppInstallStatus object.</span></span>

<span data-ttu-id="f542e-129">次の表は、userAppInstallStatus を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f542e-129">The following table shows the properties that are required when you create the userAppInstallStatus.</span></span>

|<span data-ttu-id="f542e-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f542e-130">Property</span></span>|<span data-ttu-id="f542e-131">型</span><span class="sxs-lookup"><span data-stu-id="f542e-131">Type</span></span>|<span data-ttu-id="f542e-132">説明</span><span class="sxs-lookup"><span data-stu-id="f542e-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f542e-133">ID</span><span class="sxs-lookup"><span data-stu-id="f542e-133">id</span></span>|<span data-ttu-id="f542e-134">String</span><span class="sxs-lookup"><span data-stu-id="f542e-134">String</span></span>|<span data-ttu-id="f542e-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f542e-135">Key of the entity.</span></span>|
|<span data-ttu-id="f542e-136">userName</span><span class="sxs-lookup"><span data-stu-id="f542e-136">userName</span></span>|<span data-ttu-id="f542e-137">String</span><span class="sxs-lookup"><span data-stu-id="f542e-137">String</span></span>|<span data-ttu-id="f542e-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="f542e-138">User name.</span></span>|
|<span data-ttu-id="f542e-139">userPrincipalName</span><span class="sxs-lookup"><span data-stu-id="f542e-139">userPrincipalName</span></span>|<span data-ttu-id="f542e-140">String</span><span class="sxs-lookup"><span data-stu-id="f542e-140">String</span></span>|<span data-ttu-id="f542e-141">ユーザー プリンシパル名です。</span><span class="sxs-lookup"><span data-stu-id="f542e-141">User Principal Name.</span></span>|
|<span data-ttu-id="f542e-142">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f542e-142">installedDeviceCount</span></span>|<span data-ttu-id="f542e-143">Int32</span><span class="sxs-lookup"><span data-stu-id="f542e-143">Int32</span></span>|<span data-ttu-id="f542e-144">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f542e-144">Installed Device Count.</span></span>|
|<span data-ttu-id="f542e-145">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f542e-145">failedDeviceCount</span></span>|<span data-ttu-id="f542e-146">Int32</span><span class="sxs-lookup"><span data-stu-id="f542e-146">Int32</span></span>|<span data-ttu-id="f542e-147">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f542e-147">Failed Device Count.</span></span>|
|<span data-ttu-id="f542e-148">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f542e-148">notInstalledDeviceCount</span></span>|<span data-ttu-id="f542e-149">Int32</span><span class="sxs-lookup"><span data-stu-id="f542e-149">Int32</span></span>|<span data-ttu-id="f542e-150">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f542e-150">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f542e-151">応答</span><span class="sxs-lookup"><span data-stu-id="f542e-151">Response</span></span>
<span data-ttu-id="f542e-152">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="f542e-152">If successful, this method returns a `201 Created` response code and a [userAppInstallStatus](../resources/intune-apps-userappinstallstatus.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f542e-153">例</span><span class="sxs-lookup"><span data-stu-id="f542e-153">Example</span></span>
### <a name="request"></a><span data-ttu-id="f542e-154">要求</span><span class="sxs-lookup"><span data-stu-id="f542e-154">Request</span></span>
<span data-ttu-id="f542e-155">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f542e-155">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="f542e-156">応答</span><span class="sxs-lookup"><span data-stu-id="f542e-156">Response</span></span>
<span data-ttu-id="f542e-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f542e-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





