---
title: WindowsManagementApp を更新します。
description: WindowsManagementApp オブジェクトのプロパティを更新します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 27ba9154598480972e1d7f2c9a8b5d28bb3ec4b2
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29412409"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="e3355-103">WindowsManagementApp を更新します。</span><span class="sxs-lookup"><span data-stu-id="e3355-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="e3355-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="e3355-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="e3355-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3355-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="e3355-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e3355-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e3355-107">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e3355-107">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e3355-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="e3355-108">Prerequisites</span></span>
<span data-ttu-id="e3355-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e3355-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="e3355-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e3355-111">Permission type</span></span>|<span data-ttu-id="e3355-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e3355-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e3355-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e3355-113">Delegated (work or school account)</span></span>|<span data-ttu-id="e3355-114">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="e3355-114">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="e3355-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e3355-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e3355-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3355-116">Not supported.</span></span>|
|<span data-ttu-id="e3355-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e3355-117">Application</span></span>|<span data-ttu-id="e3355-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e3355-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e3355-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e3355-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="e3355-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3355-120">Request headers</span></span>
|<span data-ttu-id="e3355-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e3355-121">Header</span></span>|<span data-ttu-id="e3355-122">値</span><span class="sxs-lookup"><span data-stu-id="e3355-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e3355-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="e3355-123">Authorization</span></span>|<span data-ttu-id="e3355-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="e3355-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e3355-125">Accept</span><span class="sxs-lookup"><span data-stu-id="e3355-125">Accept</span></span>|<span data-ttu-id="e3355-126">application/json</span><span class="sxs-lookup"><span data-stu-id="e3355-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e3355-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="e3355-127">Request body</span></span>
<span data-ttu-id="e3355-128">要求の本文に[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="e3355-128">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="e3355-129">[WindowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)を作成するときに必要なプロパティを次の表に示します。</span><span class="sxs-lookup"><span data-stu-id="e3355-129">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="e3355-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e3355-130">Property</span></span>|<span data-ttu-id="e3355-131">型</span><span class="sxs-lookup"><span data-stu-id="e3355-131">Type</span></span>|<span data-ttu-id="e3355-132">説明</span><span class="sxs-lookup"><span data-stu-id="e3355-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e3355-133">id</span><span class="sxs-lookup"><span data-stu-id="e3355-133">id</span></span>|<span data-ttu-id="e3355-134">String</span><span class="sxs-lookup"><span data-stu-id="e3355-134">String</span></span>|<span data-ttu-id="e3355-135">Windows 管理アプリケーションの一意の識別子</span><span class="sxs-lookup"><span data-stu-id="e3355-135">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="e3355-136">availableVersion</span><span class="sxs-lookup"><span data-stu-id="e3355-136">availableVersion</span></span>|<span data-ttu-id="e3355-137">String</span><span class="sxs-lookup"><span data-stu-id="e3355-137">String</span></span>|<span data-ttu-id="e3355-138">Windows 管理アプリケーションの使用可能なバージョンです。</span><span class="sxs-lookup"><span data-stu-id="e3355-138">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="e3355-139">応答</span><span class="sxs-lookup"><span data-stu-id="e3355-139">Response</span></span>
<span data-ttu-id="e3355-140">かどうかは成功すると、このメソッドが返されます、`200 OK`応答コードおよび応答の本文に更新された[windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="e3355-140">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e3355-141">例</span><span class="sxs-lookup"><span data-stu-id="e3355-141">Example</span></span>

### <a name="request"></a><span data-ttu-id="e3355-142">要求</span><span class="sxs-lookup"><span data-stu-id="e3355-142">Request</span></span>
<span data-ttu-id="e3355-143">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e3355-143">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="e3355-144">応答</span><span class="sxs-lookup"><span data-stu-id="e3355-144">Response</span></span>
<span data-ttu-id="e3355-p103">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e3355-p103">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 161

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "id": "5facc79c-c79c-5fac-9cc7-ac5f9cc7ac5f",
  "availableVersion": "Available Version value"
}
```




