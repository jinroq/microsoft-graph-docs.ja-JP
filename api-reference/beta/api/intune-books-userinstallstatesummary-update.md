---
title: userInstallStateSummary の更新
description: userInstallStateSummary オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 43401e2abe342f9947971cccbeec85a2ef92c185
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29418464"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="d73b6-103">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d73b6-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="d73b6-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="d73b6-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="d73b6-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73b6-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="d73b6-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d73b6-107">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d73b6-107">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d73b6-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="d73b6-108">Prerequisites</span></span>
<span data-ttu-id="d73b6-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d73b6-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="d73b6-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d73b6-111">Permission type</span></span>|<span data-ttu-id="d73b6-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d73b6-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d73b6-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d73b6-113">Delegated (work or school account)</span></span>|<span data-ttu-id="d73b6-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d73b6-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d73b6-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d73b6-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d73b6-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73b6-116">Not supported.</span></span>|
|<span data-ttu-id="d73b6-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d73b6-117">Application</span></span>|<span data-ttu-id="d73b6-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d73b6-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d73b6-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d73b6-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d73b6-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d73b6-120">Request headers</span></span>
|<span data-ttu-id="d73b6-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d73b6-121">Header</span></span>|<span data-ttu-id="d73b6-122">値</span><span class="sxs-lookup"><span data-stu-id="d73b6-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d73b6-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="d73b6-123">Authorization</span></span>|<span data-ttu-id="d73b6-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="d73b6-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d73b6-125">Accept</span><span class="sxs-lookup"><span data-stu-id="d73b6-125">Accept</span></span>|<span data-ttu-id="d73b6-126">application/json</span><span class="sxs-lookup"><span data-stu-id="d73b6-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d73b6-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="d73b6-127">Request body</span></span>
<span data-ttu-id="d73b6-128">要求本文で、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d73b6-128">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="d73b6-129">次の表に、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d73b6-129">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="d73b6-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d73b6-130">Property</span></span>|<span data-ttu-id="d73b6-131">型</span><span class="sxs-lookup"><span data-stu-id="d73b6-131">Type</span></span>|<span data-ttu-id="d73b6-132">説明</span><span class="sxs-lookup"><span data-stu-id="d73b6-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d73b6-133">id</span><span class="sxs-lookup"><span data-stu-id="d73b6-133">id</span></span>|<span data-ttu-id="d73b6-134">String</span><span class="sxs-lookup"><span data-stu-id="d73b6-134">String</span></span>|<span data-ttu-id="d73b6-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d73b6-135">Key of the entity.</span></span>|
|<span data-ttu-id="d73b6-136">userName</span><span class="sxs-lookup"><span data-stu-id="d73b6-136">userName</span></span>|<span data-ttu-id="d73b6-137">String</span><span class="sxs-lookup"><span data-stu-id="d73b6-137">String</span></span>|<span data-ttu-id="d73b6-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-138">User name.</span></span>|
|<span data-ttu-id="d73b6-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73b6-139">installedDeviceCount</span></span>|<span data-ttu-id="d73b6-140">Int32</span><span class="sxs-lookup"><span data-stu-id="d73b6-140">Int32</span></span>|<span data-ttu-id="d73b6-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-141">Installed Device Count.</span></span>|
|<span data-ttu-id="d73b6-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73b6-142">failedDeviceCount</span></span>|<span data-ttu-id="d73b6-143">Int32</span><span class="sxs-lookup"><span data-stu-id="d73b6-143">Int32</span></span>|<span data-ttu-id="d73b6-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-144">Failed Device Count.</span></span>|
|<span data-ttu-id="d73b6-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d73b6-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="d73b6-146">Int32</span><span class="sxs-lookup"><span data-stu-id="d73b6-146">Int32</span></span>|<span data-ttu-id="d73b6-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="d73b6-148">応答</span><span class="sxs-lookup"><span data-stu-id="d73b6-148">Response</span></span>
<span data-ttu-id="d73b6-149">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d73b6-149">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d73b6-150">例</span><span class="sxs-lookup"><span data-stu-id="d73b6-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="d73b6-151">要求</span><span class="sxs-lookup"><span data-stu-id="d73b6-151">Request</span></span>
<span data-ttu-id="d73b6-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d73b6-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d73b6-153">応答</span><span class="sxs-lookup"><span data-stu-id="d73b6-153">Response</span></span>
<span data-ttu-id="d73b6-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d73b6-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




