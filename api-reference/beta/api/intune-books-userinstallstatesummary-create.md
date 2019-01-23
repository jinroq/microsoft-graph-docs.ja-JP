---
title: userInstallStateSummary の作成
description: 新しい userInstallStateSummary オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 8dbae3b5271d271a9df1215382dbf08532fd1c22
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29413005"
---
# <a name="create-userinstallstatesummary"></a><span data-ttu-id="1907b-103">userInstallStateSummary の作成</span><span class="sxs-lookup"><span data-stu-id="1907b-103">Create userInstallStateSummary</span></span>

> <span data-ttu-id="1907b-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="1907b-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="1907b-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1907b-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="1907b-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="1907b-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="1907b-107">新しい [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="1907b-107">Create a new [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="1907b-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="1907b-108">Prerequisites</span></span>
<span data-ttu-id="1907b-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="1907b-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="1907b-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="1907b-111">Permission type</span></span>|<span data-ttu-id="1907b-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="1907b-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="1907b-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="1907b-113">Delegated (work or school account)</span></span>|<span data-ttu-id="1907b-114">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="1907b-114">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="1907b-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="1907b-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="1907b-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1907b-116">Not supported.</span></span>|
|<span data-ttu-id="1907b-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="1907b-117">Application</span></span>|<span data-ttu-id="1907b-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="1907b-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="1907b-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="1907b-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary
```

## <a name="request-headers"></a><span data-ttu-id="1907b-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1907b-120">Request headers</span></span>
|<span data-ttu-id="1907b-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="1907b-121">Header</span></span>|<span data-ttu-id="1907b-122">値</span><span class="sxs-lookup"><span data-stu-id="1907b-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="1907b-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="1907b-123">Authorization</span></span>|<span data-ttu-id="1907b-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="1907b-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="1907b-125">Accept</span><span class="sxs-lookup"><span data-stu-id="1907b-125">Accept</span></span>|<span data-ttu-id="1907b-126">application/json</span><span class="sxs-lookup"><span data-stu-id="1907b-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="1907b-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="1907b-127">Request body</span></span>
<span data-ttu-id="1907b-128">要求本文で、userInstallStateSummary オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="1907b-128">In the request body, supply a JSON representation for the userInstallStateSummary object.</span></span>

<span data-ttu-id="1907b-129">次の表に、userInstallStateSummary の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="1907b-129">The following table shows the properties that are required when you create the userInstallStateSummary.</span></span>

|<span data-ttu-id="1907b-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="1907b-130">Property</span></span>|<span data-ttu-id="1907b-131">型</span><span class="sxs-lookup"><span data-stu-id="1907b-131">Type</span></span>|<span data-ttu-id="1907b-132">説明</span><span class="sxs-lookup"><span data-stu-id="1907b-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="1907b-133">id</span><span class="sxs-lookup"><span data-stu-id="1907b-133">id</span></span>|<span data-ttu-id="1907b-134">String</span><span class="sxs-lookup"><span data-stu-id="1907b-134">String</span></span>|<span data-ttu-id="1907b-135">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="1907b-135">Key of the entity.</span></span>|
|<span data-ttu-id="1907b-136">userName</span><span class="sxs-lookup"><span data-stu-id="1907b-136">userName</span></span>|<span data-ttu-id="1907b-137">String</span><span class="sxs-lookup"><span data-stu-id="1907b-137">String</span></span>|<span data-ttu-id="1907b-138">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="1907b-138">User name.</span></span>|
|<span data-ttu-id="1907b-139">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1907b-139">installedDeviceCount</span></span>|<span data-ttu-id="1907b-140">Int32</span><span class="sxs-lookup"><span data-stu-id="1907b-140">Int32</span></span>|<span data-ttu-id="1907b-141">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="1907b-141">Installed Device Count.</span></span>|
|<span data-ttu-id="1907b-142">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1907b-142">failedDeviceCount</span></span>|<span data-ttu-id="1907b-143">Int32</span><span class="sxs-lookup"><span data-stu-id="1907b-143">Int32</span></span>|<span data-ttu-id="1907b-144">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="1907b-144">Failed Device Count.</span></span>|
|<span data-ttu-id="1907b-145">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="1907b-145">notInstalledDeviceCount</span></span>|<span data-ttu-id="1907b-146">Int32</span><span class="sxs-lookup"><span data-stu-id="1907b-146">Int32</span></span>|<span data-ttu-id="1907b-147">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="1907b-147">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="1907b-148">応答</span><span class="sxs-lookup"><span data-stu-id="1907b-148">Response</span></span>
<span data-ttu-id="1907b-149">成功した場合、このメソッドは `201 Created` 応答コードと、応答本文で [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="1907b-149">If successful, this method returns a `201 Created` response code and a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="1907b-150">例</span><span class="sxs-lookup"><span data-stu-id="1907b-150">Example</span></span>

### <a name="request"></a><span data-ttu-id="1907b-151">要求</span><span class="sxs-lookup"><span data-stu-id="1907b-151">Request</span></span>
<span data-ttu-id="1907b-152">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="1907b-152">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="1907b-153">応答</span><span class="sxs-lookup"><span data-stu-id="1907b-153">Response</span></span>
<span data-ttu-id="1907b-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="1907b-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




