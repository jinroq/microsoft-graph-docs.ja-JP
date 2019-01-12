---
title: userInstallStateSummary の作成
description: 新しい userInstallStateSummary オブジェクトを作成します。
author: tfitzmac
localization_priority: Normal
ms.prod: intune
ms.openlocfilehash: b738e79c832fbfde23bfa48a84573c6d5c8f3e98
ms.sourcegitcommit: 36be044c89a19af84c93e586e22200ec919e4c9f
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/12/2019
ms.locfileid: "27950257"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="5812c-103">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="5812c-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="5812c-104">**重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="5812c-104">**Important:** APIs under the /beta version in Microsoft Graph are in preview and are subject to change.</span></span> <span data-ttu-id="5812c-105">実稼働アプリケーションでの、これらの API の使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5812c-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="5812c-106">**注:** Intune のコントロールおよびポリシーの構成に Microsoft Graph API を使用するには、これまでどおりに顧客が Intune サービスの[適切なライセンス](https://go.microsoft.com/fwlink/?linkid=839381)を持っている必要があります。</span><span class="sxs-lookup"><span data-stu-id="5812c-106">**Note:** Using the Microsoft Graph APIs to configure Intune controls and policies still requires that the Intune service is [correctly licensed](https://go.microsoft.com/fwlink/?linkid=839381) by the customer.</span></span>

<span data-ttu-id="5812c-107">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="5812c-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>
## <a name="prerequisites"></a><span data-ttu-id="5812c-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="5812c-108">Prerequisites</span></span>
<span data-ttu-id="5812c-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="5812c-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="5812c-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="5812c-111">Permission type</span></span>|<span data-ttu-id="5812c-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="5812c-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="5812c-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="5812c-113">Delegated (work or school account)</span></span>|<span data-ttu-id="5812c-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="5812c-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="5812c-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="5812c-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="5812c-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5812c-116">Not supported.</span></span>|
|<span data-ttu-id="5812c-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="5812c-117">Application</span></span>|<span data-ttu-id="5812c-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="5812c-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="5812c-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="5812c-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="5812c-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5812c-120">Request headers</span></span>
|<span data-ttu-id="5812c-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="5812c-121">Header</span></span>|<span data-ttu-id="5812c-122">値</span><span class="sxs-lookup"><span data-stu-id="5812c-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="5812c-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="5812c-123">Authorization</span></span>|<span data-ttu-id="5812c-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="5812c-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="5812c-125">Accept</span><span class="sxs-lookup"><span data-stu-id="5812c-125">Accept</span></span>|<span data-ttu-id="5812c-126">application/json</span><span class="sxs-lookup"><span data-stu-id="5812c-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="5812c-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="5812c-127">Request body</span></span>
<span data-ttu-id="5812c-128">要求本文で、userInstallStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="5812c-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="5812c-129">次の表に、userInstallStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="5812c-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="5812c-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="5812c-130">Property</span></span>|<span data-ttu-id="5812c-131">種類</span><span class="sxs-lookup"><span data-stu-id="5812c-131">Type</span></span>|<span data-ttu-id="5812c-132">説明</span><span class="sxs-lookup"><span data-stu-id="5812c-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="5812c-133">ID</span><span class="sxs-lookup"><span data-stu-id="5812c-133">id</span></span>|<span data-ttu-id="5812c-134">String</span><span class="sxs-lookup"><span data-stu-id="5812c-134">String</span></span>|<span data-ttu-id="5812c-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="5812c-135">Key of the entity.</span></span>|
|<span data-ttu-id="5812c-136">userName</span><span class="sxs-lookup"><span data-stu-id="5812c-136">userName</span></span>|<span data-ttu-id="5812c-137">String</span><span class="sxs-lookup"><span data-stu-id="5812c-137">String</span></span>|<span data-ttu-id="5812c-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="5812c-138">User name.</span></span>|
|<span data-ttu-id="5812c-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5812c-139">installedDeviceCount</span></span>|<span data-ttu-id="5812c-140">Int32</span><span class="sxs-lookup"><span data-stu-id="5812c-140">Int32</span></span>|<span data-ttu-id="5812c-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5812c-141">Installed Device Count.</span></span>|
|<span data-ttu-id="5812c-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5812c-142">failedDeviceCount</span></span>|<span data-ttu-id="5812c-143">Int32</span><span class="sxs-lookup"><span data-stu-id="5812c-143">Int32</span></span>|<span data-ttu-id="5812c-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5812c-144">Failed Device Count.</span></span>|
|<span data-ttu-id="5812c-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="5812c-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="5812c-146">Int32</span><span class="sxs-lookup"><span data-stu-id="5812c-146">Int32</span></span>|<span data-ttu-id="5812c-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="5812c-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="5812c-148">応答</span><span class="sxs-lookup"><span data-stu-id="5812c-148">Response</span></span>
<span data-ttu-id="5812c-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="5812c-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="5812c-150">例</span><span class="sxs-lookup"><span data-stu-id="5812c-150">Example</span></span>
### <a name="request"></a><span data-ttu-id="5812c-151">要求</span><span class="sxs-lookup"><span data-stu-id="5812c-151">Request</span></span>
<span data-ttu-id="5812c-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="5812c-152">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
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

### <a name="response"></a><span data-ttu-id="5812c-153">応答</span><span class="sxs-lookup"><span data-stu-id="5812c-153">Response</span></span>
<span data-ttu-id="5812c-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="5812c-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





