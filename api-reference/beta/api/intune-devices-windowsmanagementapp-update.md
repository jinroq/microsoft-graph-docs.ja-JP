---
title: WindowsManagementApp の更新
description: WindowsManagementApp オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
doc_type: apiPageType
ms.openlocfilehash: a8c3718274fad980e9b0b2b7b0d227e99dcd9428
ms.sourcegitcommit: 2c62457e57467b8d50f21b255b553106a9a5d8d6
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 07/31/2019
ms.locfileid: "35981242"
---
# <a name="update-windowsmanagementapp"></a><span data-ttu-id="f9287-103">WindowsManagementApp の更新</span><span class="sxs-lookup"><span data-stu-id="f9287-103">Update windowsManagementApp</span></span>

> <span data-ttu-id="f9287-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9287-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="f9287-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9287-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="f9287-106">[Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="f9287-106">Update the properties of a [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="f9287-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="f9287-107">Prerequisites</span></span>
<span data-ttu-id="f9287-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="f9287-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="f9287-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="f9287-110">Permission type</span></span>|<span data-ttu-id="f9287-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="f9287-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="f9287-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="f9287-112">Delegated (work or school account)</span></span>|<span data-ttu-id="f9287-113">DeviceManagementManagedDevices.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="f9287-113">DeviceManagementManagedDevices.ReadWrite.All</span></span>|
|<span data-ttu-id="f9287-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="f9287-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="f9287-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9287-115">Not supported.</span></span>|
|<span data-ttu-id="f9287-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="f9287-116">Application</span></span>|<span data-ttu-id="f9287-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="f9287-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="f9287-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="f9287-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceAppManagement/windowsManagementApp
```

## <a name="request-headers"></a><span data-ttu-id="f9287-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9287-119">Request headers</span></span>
|<span data-ttu-id="f9287-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="f9287-120">Header</span></span>|<span data-ttu-id="f9287-121">値</span><span class="sxs-lookup"><span data-stu-id="f9287-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="f9287-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="f9287-122">Authorization</span></span>|<span data-ttu-id="f9287-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="f9287-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="f9287-124">承諾</span><span class="sxs-lookup"><span data-stu-id="f9287-124">Accept</span></span>|<span data-ttu-id="f9287-125">application/json</span><span class="sxs-lookup"><span data-stu-id="f9287-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="f9287-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="f9287-126">Request body</span></span>
<span data-ttu-id="f9287-127">要求本文で、 [Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="f9287-127">In the request body, supply a JSON representation for the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object.</span></span>

<span data-ttu-id="f9287-128">次の表に、 [Windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="f9287-128">The following table shows the properties that are required when you create the [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md).</span></span>

|<span data-ttu-id="f9287-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="f9287-129">Property</span></span>|<span data-ttu-id="f9287-130">型</span><span class="sxs-lookup"><span data-stu-id="f9287-130">Type</span></span>|<span data-ttu-id="f9287-131">説明</span><span class="sxs-lookup"><span data-stu-id="f9287-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="f9287-132">id</span><span class="sxs-lookup"><span data-stu-id="f9287-132">id</span></span>|<span data-ttu-id="f9287-133">String</span><span class="sxs-lookup"><span data-stu-id="f9287-133">String</span></span>|<span data-ttu-id="f9287-134">Windows management アプリの一意識別子</span><span class="sxs-lookup"><span data-stu-id="f9287-134">Unique Identifier for the Windows management app</span></span>|
|<span data-ttu-id="f9287-135">プロパティ availableversion</span><span class="sxs-lookup"><span data-stu-id="f9287-135">availableVersion</span></span>|<span data-ttu-id="f9287-136">String</span><span class="sxs-lookup"><span data-stu-id="f9287-136">String</span></span>|<span data-ttu-id="f9287-137">Windows management アプリの利用可能なバージョン。</span><span class="sxs-lookup"><span data-stu-id="f9287-137">Windows management app available version.</span></span>|



## <a name="response"></a><span data-ttu-id="f9287-138">応答</span><span class="sxs-lookup"><span data-stu-id="f9287-138">Response</span></span>
<span data-ttu-id="f9287-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[windowsmanagementapp](../resources/intune-devices-windowsmanagementapp.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="f9287-139">If successful, this method returns a `200 OK` response code and an updated [windowsManagementApp](../resources/intune-devices-windowsmanagementapp.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="f9287-140">例</span><span class="sxs-lookup"><span data-stu-id="f9287-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="f9287-141">要求</span><span class="sxs-lookup"><span data-stu-id="f9287-141">Request</span></span>
<span data-ttu-id="f9287-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="f9287-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceAppManagement/windowsManagementApp
Content-type: application/json
Content-length: 112

{
  "@odata.type": "#microsoft.graph.windowsManagementApp",
  "availableVersion": "Available Version value"
}
```

### <a name="response"></a><span data-ttu-id="f9287-143">応答</span><span class="sxs-lookup"><span data-stu-id="f9287-143">Response</span></span>
<span data-ttu-id="f9287-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="f9287-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
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





