---
title: userInstallStateSummary の更新
description: userInstallStateSummary オブジェクトのプロパティを更新します。
author: tfitzmac
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: a924db2f3dd97921eddd3c092c60c7f87e1b8b12
ms.sourcegitcommit: 7b98b61db7cdbaff037e1b222ac58eef4c5bee89
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 03/29/2019
ms.locfileid: "30985908"
---
# <a name="update-userinstallstatesummary"></a><span data-ttu-id="d93d8-103">userInstallStateSummary の更新</span><span class="sxs-lookup"><span data-stu-id="d93d8-103">Update userInstallStateSummary</span></span>

> <span data-ttu-id="d93d8-104">**重要:** ベータ版の Microsoft Graph api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d93d8-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="d93d8-105">**注:** Microsoft graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="d93d8-106">[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="d93d8-106">Update the properties of a [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="d93d8-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="d93d8-107">Prerequisites</span></span>
<span data-ttu-id="d93d8-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="d93d8-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="d93d8-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="d93d8-110">Permission type</span></span>|<span data-ttu-id="d93d8-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="d93d8-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="d93d8-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="d93d8-112">Delegated (work or school account)</span></span>|<span data-ttu-id="d93d8-113">DeviceManagementApps.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="d93d8-113">DeviceManagementApps.ReadWrite.All</span></span>|
|<span data-ttu-id="d93d8-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="d93d8-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="d93d8-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d93d8-115">Not supported.</span></span>|
|<span data-ttu-id="d93d8-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="d93d8-116">Application</span></span>|<span data-ttu-id="d93d8-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="d93d8-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="d93d8-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="d93d8-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/managedEBooks/{managedEBookId}/userStateSummary/{userInstallStateSummaryId}
```

## <a name="request-headers"></a><span data-ttu-id="d93d8-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d93d8-119">Request headers</span></span>
|<span data-ttu-id="d93d8-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="d93d8-120">Header</span></span>|<span data-ttu-id="d93d8-121">値</span><span class="sxs-lookup"><span data-stu-id="d93d8-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="d93d8-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="d93d8-122">Authorization</span></span>|<span data-ttu-id="d93d8-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="d93d8-124">承諾</span><span class="sxs-lookup"><span data-stu-id="d93d8-124">Accept</span></span>|<span data-ttu-id="d93d8-125">application/json</span><span class="sxs-lookup"><span data-stu-id="d93d8-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="d93d8-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="d93d8-126">Request body</span></span>
<span data-ttu-id="d93d8-127">要求本文で、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="d93d8-127">In the request body, supply a JSON representation for the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object.</span></span>

<span data-ttu-id="d93d8-128">次の表に、[userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="d93d8-128">The following table shows the properties that are required when you create the [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md).</span></span>

|<span data-ttu-id="d93d8-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="d93d8-129">Property</span></span>|<span data-ttu-id="d93d8-130">型</span><span class="sxs-lookup"><span data-stu-id="d93d8-130">Type</span></span>|<span data-ttu-id="d93d8-131">説明</span><span class="sxs-lookup"><span data-stu-id="d93d8-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="d93d8-132">id</span><span class="sxs-lookup"><span data-stu-id="d93d8-132">id</span></span>|<span data-ttu-id="d93d8-133">String</span><span class="sxs-lookup"><span data-stu-id="d93d8-133">String</span></span>|<span data-ttu-id="d93d8-134">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="d93d8-134">Key of the entity.</span></span>|
|<span data-ttu-id="d93d8-135">userName</span><span class="sxs-lookup"><span data-stu-id="d93d8-135">userName</span></span>|<span data-ttu-id="d93d8-136">String</span><span class="sxs-lookup"><span data-stu-id="d93d8-136">String</span></span>|<span data-ttu-id="d93d8-137">ユーザー名です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-137">User name.</span></span>|
|<span data-ttu-id="d93d8-138">installedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d93d8-138">installedDeviceCount</span></span>|<span data-ttu-id="d93d8-139">Int32</span><span class="sxs-lookup"><span data-stu-id="d93d8-139">Int32</span></span>|<span data-ttu-id="d93d8-140">インストールされたデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-140">Installed Device Count.</span></span>|
|<span data-ttu-id="d93d8-141">failedDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d93d8-141">failedDeviceCount</span></span>|<span data-ttu-id="d93d8-142">Int32</span><span class="sxs-lookup"><span data-stu-id="d93d8-142">Int32</span></span>|<span data-ttu-id="d93d8-143">失敗したデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-143">Failed Device Count.</span></span>|
|<span data-ttu-id="d93d8-144">notInstalledDeviceCount</span><span class="sxs-lookup"><span data-stu-id="d93d8-144">notInstalledDeviceCount</span></span>|<span data-ttu-id="d93d8-145">Int32</span><span class="sxs-lookup"><span data-stu-id="d93d8-145">Int32</span></span>|<span data-ttu-id="d93d8-146">インストールされていないデバイスの数です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-146">Not installed device count.</span></span>|



## <a name="response"></a><span data-ttu-id="d93d8-147">応答</span><span class="sxs-lookup"><span data-stu-id="d93d8-147">Response</span></span>
<span data-ttu-id="d93d8-148">成功した場合、このメソッドは `200 OK` 応答コードと、応答本文で更新された [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="d93d8-148">If successful, this method returns a `200 OK` response code and an updated [userInstallStateSummary](../resources/intune-books-userinstallstatesummary.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="d93d8-149">例</span><span class="sxs-lookup"><span data-stu-id="d93d8-149">Example</span></span>

### <a name="request"></a><span data-ttu-id="d93d8-150">要求</span><span class="sxs-lookup"><span data-stu-id="d93d8-150">Request</span></span>
<span data-ttu-id="d93d8-151">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="d93d8-151">Here is an example of the request.</span></span>
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

### <a name="response"></a><span data-ttu-id="d93d8-152">応答</span><span class="sxs-lookup"><span data-stu-id="d93d8-152">Response</span></span>
<span data-ttu-id="d93d8-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="d93d8-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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




