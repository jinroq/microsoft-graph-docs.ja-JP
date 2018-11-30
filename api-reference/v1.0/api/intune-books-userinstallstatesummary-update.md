---
title: userInstallStateSummary の更新
description: userInstallStateSummary オブジェクトのプロパティを更新します。
ms.openlocfilehash: a5c3f1278a8c9696b65663eaaeafcb76e1e09840
ms.sourcegitcommit: 334e84b4aed63162bcc31831cffd6d363dafee02
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 11/29/2018
ms.locfileid: "27020332"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="7410e-103">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="7410e-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="7410e-104">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="7410e-104">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="7410e-105">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="7410e-105">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="7410e-106">前提条件</span><span class="sxs-lookup"><span data-stu-id="7410e-106">Prerequisites</span></span>
<span data-ttu-id="7410e-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="7410e-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="7410e-109">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="7410e-109">Permission type</span></span>|<span data-ttu-id="7410e-110">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="7410e-110">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="7410e-111">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="7410e-111">Delegated (work or school account)</span></span>|<span data-ttu-id="7410e-112">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="7410e-112">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="7410e-113">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="7410e-113">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="7410e-114">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7410e-114">Not supported.</span></span>|
|<span data-ttu-id="7410e-115">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="7410e-115">Application</span></span>|<span data-ttu-id="7410e-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="7410e-116">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="7410e-117">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="7410e-117">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="7410e-118">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7410e-118">Request headers</span></span>
|<span data-ttu-id="7410e-119">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="7410e-119">Header</span></span>|<span data-ttu-id="7410e-120">値</span><span class="sxs-lookup"><span data-stu-id="7410e-120">Value</span></span>|
|:---|:---|
|<span data-ttu-id="7410e-121">Authorization</span><span class="sxs-lookup"><span data-stu-id="7410e-121">Authorization</span></span>|<span data-ttu-id="7410e-122">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="7410e-122">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="7410e-123">Accept</span><span class="sxs-lookup"><span data-stu-id="7410e-123">Accept</span></span>|<span data-ttu-id="7410e-124">application/json</span><span class="sxs-lookup"><span data-stu-id="7410e-124">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="7410e-125">要求本文</span><span class="sxs-lookup"><span data-stu-id="7410e-125">Request body</span></span>
<span data-ttu-id="7410e-126">要求本文で、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="7410e-126">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="7410e-127">次の表に、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="7410e-127">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="7410e-128">プロパティ</span><span class="sxs-lookup"><span data-stu-id="7410e-128">Property</span></span>|<span data-ttu-id="7410e-129">型</span><span class="sxs-lookup"><span data-stu-id="7410e-129">Type</span></span>|<span data-ttu-id="7410e-130">説明</span><span class="sxs-lookup"><span data-stu-id="7410e-130">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="7410e-131">id</span><span class="sxs-lookup"><span data-stu-id="7410e-131">id</span></span>|<span data-ttu-id="7410e-132">String</span><span class="sxs-lookup"><span data-stu-id="7410e-132">String</span></span>|<span data-ttu-id="7410e-133">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="7410e-133">Key of the entity.</span></span>|
|<span data-ttu-id="7410e-134">userName</span><span class="sxs-lookup"><span data-stu-id="7410e-134">userName</span></span>|<span data-ttu-id="7410e-135">String</span><span class="sxs-lookup"><span data-stu-id="7410e-135">String</span></span>|<span data-ttu-id="7410e-136">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="7410e-136">User name.</span></span>|
|<span data-ttu-id="7410e-137">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7410e-137">installedDeviceCount</span></span>|<span data-ttu-id="7410e-138">Int32</span><span class="sxs-lookup"><span data-stu-id="7410e-138">Int32</span></span>|<span data-ttu-id="7410e-139">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7410e-139">Installed Device Count.</span></span>|
|<span data-ttu-id="7410e-140">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7410e-140">failedDeviceCount</span></span>|<span data-ttu-id="7410e-141">Int32</span><span class="sxs-lookup"><span data-stu-id="7410e-141">Int32</span></span>|<span data-ttu-id="7410e-142">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7410e-142">Failed Device Count.</span></span>|
|<span data-ttu-id="7410e-143">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="7410e-143">notInstalledDeviceCount</span></span>|<span data-ttu-id="7410e-144">Int32</span><span class="sxs-lookup"><span data-stu-id="7410e-144">Int32</span></span>|<span data-ttu-id="7410e-145">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="7410e-145">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="7410e-146">応答</span><span class="sxs-lookup"><span data-stu-id="7410e-146">Response</span></span>
<span data-ttu-id="7410e-147">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="7410e-147">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="7410e-148">例</span><span class="sxs-lookup"><span data-stu-id="7410e-148">Example</span></span>
### <a name="request"></a><span data-ttu-id="7410e-149">要求</span><span class="sxs-lookup"><span data-stu-id="7410e-149">Request</span></span>
<span data-ttu-id="7410e-150">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="7410e-150">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/v1.0/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="7410e-151">応答</span><span class="sxs-lookup"><span data-stu-id="7410e-151">Response</span></span>
<span data-ttu-id="7410e-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="7410e-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
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



