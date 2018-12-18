---
title: userInstallStateSummary の作成
description: 新しい userInstallStateSummary オブジェクトを作成します。
author: tfitzmac
ms.openlocfilehash: a1da2855896bae9d9c902ae978d3ce8c127f3bc4
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27318418"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="727a8-103">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="727a8-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="727a8-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="727a8-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="727a8-105">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="727a8-105">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="727a8-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="727a8-106">Prerequisites</span></span>
<span data-ttu-id="727a8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="727a8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="727a8-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="727a8-109">Permission type</span></span>|<span data-ttu-id="727a8-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="727a8-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="727a8-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="727a8-111">Delegated (work or school account)</span></span>|<span data-ttu-id="727a8-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="727a8-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="727a8-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="727a8-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="727a8-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="727a8-114">Not supported.</span></span>|
|<span data-ttu-id="727a8-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="727a8-115">Application</span></span>|<span data-ttu-id="727a8-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="727a8-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="727a8-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="727a8-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="727a8-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="727a8-118">Request headers</span></span>
|<span data-ttu-id="727a8-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="727a8-119">Header</span></span>|<span data-ttu-id="727a8-120">値</span><span class="sxs-lookup"><span data-stu-id="727a8-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="727a8-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="727a8-121">Authorization</span></span>|<span data-ttu-id="727a8-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="727a8-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="727a8-123">Accept</span><span class="sxs-lookup"><span data-stu-id="727a8-123">Accept</span></span>|<span data-ttu-id="727a8-124">application/json</span><span class="sxs-lookup"><span data-stu-id="727a8-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="727a8-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="727a8-125">Request body</span></span>
<span data-ttu-id="727a8-126">要求本文で、userInstallStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="727a8-126">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="727a8-127">次の表に、userInstallStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="727a8-127">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="727a8-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="727a8-128">Property</span></span>|<span data-ttu-id="727a8-129">種類</span><span class="sxs-lookup"><span data-stu-id="727a8-129">Type</span></span>|<span data-ttu-id="727a8-130">説明</span><span class="sxs-lookup"><span data-stu-id="727a8-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="727a8-131">ID</span><span class="sxs-lookup"><span data-stu-id="727a8-131">id</span></span>|<span data-ttu-id="727a8-132">String</span><span class="sxs-lookup"><span data-stu-id="727a8-132">String</span></span>|<span data-ttu-id="727a8-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="727a8-133">Key of the entity.</span></span>|
|<span data-ttu-id="727a8-134">userName</span><span class="sxs-lookup"><span data-stu-id="727a8-134">userName</span></span>|<span data-ttu-id="727a8-135">String</span><span class="sxs-lookup"><span data-stu-id="727a8-135">String</span></span>|<span data-ttu-id="727a8-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="727a8-136">User name.</span></span>|
|<span data-ttu-id="727a8-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="727a8-137">installedDeviceCount</span></span>|<span data-ttu-id="727a8-138">Int32</span><span class="sxs-lookup"><span data-stu-id="727a8-138">Int32</span></span>|<span data-ttu-id="727a8-139">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="727a8-139">Installed Device Count.</span></span>|
|<span data-ttu-id="727a8-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="727a8-140">failedDeviceCount</span></span>|<span data-ttu-id="727a8-141">Int32</span><span class="sxs-lookup"><span data-stu-id="727a8-141">Int32</span></span>|<span data-ttu-id="727a8-142">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="727a8-142">Failed Device Count.</span></span>|
|<span data-ttu-id="727a8-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="727a8-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="727a8-144">Int32</span><span class="sxs-lookup"><span data-stu-id="727a8-144">Int32</span></span>|<span data-ttu-id="727a8-145">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="727a8-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="727a8-146">応答</span><span class="sxs-lookup"><span data-stu-id="727a8-146">Response</span></span>
<span data-ttu-id="727a8-147">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="727a8-147">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="727a8-148">例</span><span class="sxs-lookup"><span data-stu-id="727a8-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="727a8-149">要求</span><span class="sxs-lookup"><span data-stu-id="727a8-149">Request</span></span>
<span data-ttu-id="727a8-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="727a8-150">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="727a8-151">応答</span><span class="sxs-lookup"><span data-stu-id="727a8-151">Response</span></span>
<span data-ttu-id="727a8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="727a8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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



