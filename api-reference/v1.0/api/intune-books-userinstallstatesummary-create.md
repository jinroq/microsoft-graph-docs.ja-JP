---
title: userInstallStateSummary の作成
description: 新しい userInstallStateSummary オブジェクトを作成します。
ms.openlocfilehash: d524801d8ee1b44ea955afdeb2a7c78364d89360
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27023928"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="45de9-103">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="45de9-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="45de9-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="45de9-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="45de9-105">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="45de9-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="45de9-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="45de9-106">Prerequisites</span></span>
<span data-ttu-id="45de9-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="45de9-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="45de9-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="45de9-109">Permission type</span></span>|<span data-ttu-id="45de9-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="45de9-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="45de9-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="45de9-111">Delegated (work or school account)</span></span>|<span data-ttu-id="45de9-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="45de9-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="45de9-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="45de9-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="45de9-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45de9-114">Not supported.</span></span>|
|<span data-ttu-id="45de9-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="45de9-115">Application</span></span>|<span data-ttu-id="45de9-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="45de9-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="45de9-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="45de9-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="45de9-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45de9-118">Request headers</span></span>
|<span data-ttu-id="45de9-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="45de9-119">Header</span></span>|<span data-ttu-id="45de9-120">値</span><span class="sxs-lookup"><span data-stu-id="45de9-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="45de9-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="45de9-121">Authorization</span></span>|<span data-ttu-id="45de9-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="45de9-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="45de9-123">Accept</span><span class="sxs-lookup"><span data-stu-id="45de9-123">Accept</span></span>|<span data-ttu-id="45de9-124">application/json</span><span class="sxs-lookup"><span data-stu-id="45de9-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="45de9-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="45de9-125">Request body</span></span>
<span data-ttu-id="45de9-126">要求本文で、userInstallStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="45de9-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="45de9-127">次の表に、userInstallStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="45de9-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="45de9-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="45de9-128">Property</span></span>|<span data-ttu-id="45de9-129">型</span><span class="sxs-lookup"><span data-stu-id="45de9-129">Type</span></span>|<span data-ttu-id="45de9-130">説明</span><span class="sxs-lookup"><span data-stu-id="45de9-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="45de9-131">id</span><span class="sxs-lookup"><span data-stu-id="45de9-131">id</span></span>|<span data-ttu-id="45de9-132">String</span><span class="sxs-lookup"><span data-stu-id="45de9-132">String</span></span>|<span data-ttu-id="45de9-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="45de9-133">Key of the entity.</span></span>|
|<span data-ttu-id="45de9-134">userName</span><span class="sxs-lookup"><span data-stu-id="45de9-134">userName</span></span>|<span data-ttu-id="45de9-135">String</span><span class="sxs-lookup"><span data-stu-id="45de9-135">String</span></span>|<span data-ttu-id="45de9-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="45de9-136">User name.</span></span>|
|<span data-ttu-id="45de9-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45de9-137">installedDeviceCount</span></span>|<span data-ttu-id="45de9-138">Int32</span><span class="sxs-lookup"><span data-stu-id="45de9-138">Int32</span></span>|<span data-ttu-id="45de9-139">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45de9-139">Installed Device Count.</span></span>|
|<span data-ttu-id="45de9-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45de9-140">failedDeviceCount</span></span>|<span data-ttu-id="45de9-141">Int32</span><span class="sxs-lookup"><span data-stu-id="45de9-141">Int32</span></span>|<span data-ttu-id="45de9-142">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45de9-142">Failed Device Count.</span></span>|
|<span data-ttu-id="45de9-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="45de9-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="45de9-144">Int32</span><span class="sxs-lookup"><span data-stu-id="45de9-144">Int32</span></span>|<span data-ttu-id="45de9-145">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="45de9-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="45de9-146">応答</span><span class="sxs-lookup"><span data-stu-id="45de9-146">Response</span></span>
<span data-ttu-id="45de9-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="45de9-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="45de9-148">例</span><span class="sxs-lookup"><span data-stu-id="45de9-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="45de9-149">要求</span><span class="sxs-lookup"><span data-stu-id="45de9-149">Request</span></span>
<span data-ttu-id="45de9-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="45de9-150">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
Content-type: application/json
Content-length: 189

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="45de9-151">応答</span><span class="sxs-lookup"><span data-stu-id="45de9-151">Response</span></span>
<span data-ttu-id="45de9-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="45de9-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 238

{
  "@odata.type": "#microsoft.graph.userInstallStateSummary",
  "id": "1e5b41ba-41ba-1e5b-ba41-5b1eba415b1e",
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```



