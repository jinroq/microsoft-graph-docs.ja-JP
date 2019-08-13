---
title: userInstallStateSummary の更新
description: userInstallStateSummary オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: caca487dcb87af6f0b33309d06007551104e99d0
ms.sourcegitcommit: b5425ebf648572569b032ded5b56e1dcf3830515
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 08/13/2019
ms.locfileid: "36328284"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="f9594-103">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="f9594-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="f9594-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9594-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9594-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9594-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9594-106">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9594-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9594-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9594-107">Prerequisites</span></span>
<span data-ttu-id="f9594-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9594-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9594-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9594-110">Permission type</span></span>|<span data-ttu-id="f9594-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9594-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9594-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9594-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9594-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9594-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="f9594-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9594-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9594-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9594-115">Not supported.</span></span>|
|<span data-ttu-id="f9594-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9594-116">Application</span></span>|<span data-ttu-id="f9594-117">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9594-117">DeviceManagementApps.ReadWrite.All</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9594-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9594-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="f9594-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9594-119">Request headers</span></span>
|<span data-ttu-id="f9594-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9594-120">Header</span></span>|<span data-ttu-id="f9594-121">値</span><span class="sxs-lookup"><span data-stu-id="f9594-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9594-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9594-122">Authorization</span></span>|<span data-ttu-id="f9594-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9594-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9594-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f9594-124">Accept</span></span>|<span data-ttu-id="f9594-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9594-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9594-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9594-126">Request body</span></span>
<span data-ttu-id="f9594-127">要求本文で、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9594-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="f9594-128">次の表に、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9594-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="f9594-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9594-129">Property</span></span>|<span data-ttu-id="f9594-130">型</span><span class="sxs-lookup"><span data-stu-id="f9594-130">Type</span></span>|<span data-ttu-id="f9594-131">説明</span><span class="sxs-lookup"><span data-stu-id="f9594-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9594-132">id</span><span class="sxs-lookup"><span data-stu-id="f9594-132">id</span></span>|<span data-ttu-id="f9594-133">String</span><span class="sxs-lookup"><span data-stu-id="f9594-133">String</span></span>|<span data-ttu-id="f9594-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="f9594-134">Key of the entity.</span></span>|
|<span data-ttu-id="f9594-135">userName</span><span class="sxs-lookup"><span data-stu-id="f9594-135">userName</span></span>|<span data-ttu-id="f9594-136">String</span><span class="sxs-lookup"><span data-stu-id="f9594-136">String</span></span>|<span data-ttu-id="f9594-137">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="f9594-137">User name.</span></span>|
|<span data-ttu-id="f9594-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9594-138">installedDeviceCount</span></span>|<span data-ttu-id="f9594-139">Int32</span><span class="sxs-lookup"><span data-stu-id="f9594-139">Int32</span></span>|<span data-ttu-id="f9594-140">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f9594-140">Installed Device Count.</span></span>|
|<span data-ttu-id="f9594-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9594-141">failedDeviceCount</span></span>|<span data-ttu-id="f9594-142">Int32</span><span class="sxs-lookup"><span data-stu-id="f9594-142">Int32</span></span>|<span data-ttu-id="f9594-143">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f9594-143">Failed Device Count.</span></span>|
|<span data-ttu-id="f9594-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="f9594-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="f9594-145">Int32</span><span class="sxs-lookup"><span data-stu-id="f9594-145">Int32</span></span>|<span data-ttu-id="f9594-146">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="f9594-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="f9594-147">応答</span><span class="sxs-lookup"><span data-stu-id="f9594-147">Response</span></span>
<span data-ttu-id="f9594-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9594-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9594-149">例</span><span class="sxs-lookup"><span data-stu-id="f9594-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9594-150">要求</span><span class="sxs-lookup"><span data-stu-id="f9594-150">Request</span></span>
<span data-ttu-id="f9594-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9594-151">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
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

### <a name="response"></a><span data-ttu-id="f9594-152">応答</span><span class="sxs-lookup"><span data-stu-id="f9594-152">Response</span></span>
<span data-ttu-id="f9594-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9594-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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






