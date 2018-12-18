---
title: userInstallStateSummary の更新
description: userInstallStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
ms.openlocfilehash: 10129a9a18030498add1b8e3c0b664f2aa921de6
ms.sourcegitcommit: 6a82bf240a3cfc0baabd227349e08a08311e3d44
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 12/18/2018
ms.locfileid: "27316465"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="3eace-103">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="3eace-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="3eace-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="3eace-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="3eace-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eace-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="3eace-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="3eace-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="3eace-107">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="3eace-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="3eace-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="3eace-108">Prerequisites</span></span>
<span data-ttu-id="3eace-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="3eace-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="3eace-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="3eace-111">Permission type</span></span>|<span data-ttu-id="3eace-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="3eace-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="3eace-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="3eace-113">Delegated (work or school account)</span></span>|<span data-ttu-id="3eace-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="3eace-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="3eace-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="3eace-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="3eace-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eace-116">Not supported.</span></span>|
|<span data-ttu-id="3eace-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="3eace-117">Application</span></span>|<span data-ttu-id="3eace-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="3eace-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="3eace-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="3eace-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="3eace-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3eace-120">Request headers</span></span>
|<span data-ttu-id="3eace-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="3eace-121">Header</span></span>|<span data-ttu-id="3eace-122">値</span><span class="sxs-lookup"><span data-stu-id="3eace-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="3eace-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="3eace-123">Authorization</span></span>|<span data-ttu-id="3eace-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="3eace-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="3eace-125">Accept</span><span class="sxs-lookup"><span data-stu-id="3eace-125">Accept</span></span>|<span data-ttu-id="3eace-126">application/json</span><span class="sxs-lookup"><span data-stu-id="3eace-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="3eace-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="3eace-127">Request body</span></span>
<span data-ttu-id="3eace-128">要求本文で、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="3eace-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="3eace-129">次の表に、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="3eace-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="3eace-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="3eace-130">Property</span></span>|<span data-ttu-id="3eace-131">種類</span><span class="sxs-lookup"><span data-stu-id="3eace-131">Type</span></span>|<span data-ttu-id="3eace-132">説明</span><span class="sxs-lookup"><span data-stu-id="3eace-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="3eace-133">ID</span><span class="sxs-lookup"><span data-stu-id="3eace-133">id</span></span>|<span data-ttu-id="3eace-134">String</span><span class="sxs-lookup"><span data-stu-id="3eace-134">String</span></span>|<span data-ttu-id="3eace-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="3eace-135">Key of the entity.</span></span>|
|<span data-ttu-id="3eace-136">userName</span><span class="sxs-lookup"><span data-stu-id="3eace-136">userName</span></span>|<span data-ttu-id="3eace-137">String</span><span class="sxs-lookup"><span data-stu-id="3eace-137">String</span></span>|<span data-ttu-id="3eace-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="3eace-138">User name.</span></span>|
|<span data-ttu-id="3eace-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3eace-139">installedDeviceCount</span></span>|<span data-ttu-id="3eace-140">Int32</span><span class="sxs-lookup"><span data-stu-id="3eace-140">Int32</span></span>|<span data-ttu-id="3eace-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3eace-141">Installed Device Count.</span></span>|
|<span data-ttu-id="3eace-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3eace-142">failedDeviceCount</span></span>|<span data-ttu-id="3eace-143">Int32</span><span class="sxs-lookup"><span data-stu-id="3eace-143">Int32</span></span>|<span data-ttu-id="3eace-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3eace-144">Failed Device Count.</span></span>|
|<span data-ttu-id="3eace-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="3eace-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="3eace-146">Int32</span><span class="sxs-lookup"><span data-stu-id="3eace-146">Int32</span></span>|<span data-ttu-id="3eace-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="3eace-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="3eace-148">応答</span><span class="sxs-lookup"><span data-stu-id="3eace-148">Response</span></span>
<span data-ttu-id="3eace-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="3eace-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="3eace-150">例</span><span class="sxs-lookup"><span data-stu-id="3eace-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="3eace-151">要求</span><span class="sxs-lookup"><span data-stu-id="3eace-151">Request</span></span>
<span data-ttu-id="3eace-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="3eace-152">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
Content-type: application/json
Content-length: 127

{
  "userName": "User Name value",
  "installedDeviceCount": 4,
  "failedDeviceCount": 1,
  "notInstalledDeviceCount": 7
}
```

### <a name="response"></a><span data-ttu-id="3eace-153">応答</span><span class="sxs-lookup"><span data-stu-id="3eace-153">Response</span></span>
<span data-ttu-id="3eace-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="3eace-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





