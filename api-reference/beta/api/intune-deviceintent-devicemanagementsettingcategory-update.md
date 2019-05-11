---
title: DeviceManagementSettingCategory の更新
description: DeviceManagementSettingCategory オブジェクトのプロパティを更新します。
author: rolyon
localization_priority: Normal
ms.prod: Intune
ms.openlocfilehash: 1ce6959714bebbeb26c69ae0afcfd74f75633615
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33915719"
---
# <a name="update-devicemanagementsettingcategory"></a><span data-ttu-id="4c4b6-103">DeviceManagementSettingCategory の更新</span><span class="sxs-lookup"><span data-stu-id="4c4b6-103">Update deviceManagementSettingCategory</span></span>

> <span data-ttu-id="4c4b6-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="4c4b6-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="4c4b6-106">[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-106">Update the properties of a [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="4c4b6-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="4c4b6-107">Prerequisites</span></span>
<span data-ttu-id="4c4b6-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="4c4b6-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="4c4b6-110">Permission type</span></span>|<span data-ttu-id="4c4b6-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="4c4b6-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="4c4b6-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="4c4b6-112">Delegated (work or school account)</span></span>|<span data-ttu-id="4c4b6-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="4c4b6-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="4c4b6-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="4c4b6-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="4c4b6-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-115">Not supported.</span></span>|
|<span data-ttu-id="4c4b6-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="4c4b6-116">Application</span></span>|<span data-ttu-id="4c4b6-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="4c4b6-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="4c4b6-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /deviceManagement/categories/{deviceManagementSettingCategoryId}
```

## <a name="request-headers"></a><span data-ttu-id="4c4b6-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c4b6-119">Request headers</span></span>
|<span data-ttu-id="4c4b6-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="4c4b6-120">Header</span></span>|<span data-ttu-id="4c4b6-121">値</span><span class="sxs-lookup"><span data-stu-id="4c4b6-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="4c4b6-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="4c4b6-122">Authorization</span></span>|<span data-ttu-id="4c4b6-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="4c4b6-124">承諾</span><span class="sxs-lookup"><span data-stu-id="4c4b6-124">Accept</span></span>|<span data-ttu-id="4c4b6-125">application/json</span><span class="sxs-lookup"><span data-stu-id="4c4b6-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="4c4b6-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="4c4b6-126">Request body</span></span>
<span data-ttu-id="4c4b6-127">要求本文で、 [Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-127">In the request body, supply a JSON representation for the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object.</span></span>

<span data-ttu-id="4c4b6-128">次の表に、 [Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-128">The following table shows the properties that are required when you create the [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md).</span></span>

|<span data-ttu-id="4c4b6-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="4c4b6-129">Property</span></span>|<span data-ttu-id="4c4b6-130">型</span><span class="sxs-lookup"><span data-stu-id="4c4b6-130">Type</span></span>|<span data-ttu-id="4c4b6-131">説明</span><span class="sxs-lookup"><span data-stu-id="4c4b6-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="4c4b6-132">id</span><span class="sxs-lookup"><span data-stu-id="4c4b6-132">id</span></span>|<span data-ttu-id="4c4b6-133">文字列</span><span class="sxs-lookup"><span data-stu-id="4c4b6-133">String</span></span>|<span data-ttu-id="4c4b6-134">カテゴリ ID</span><span class="sxs-lookup"><span data-stu-id="4c4b6-134">The category ID</span></span>|
|<span data-ttu-id="4c4b6-135">displayName</span><span class="sxs-lookup"><span data-stu-id="4c4b6-135">displayName</span></span>|<span data-ttu-id="4c4b6-136">String</span><span class="sxs-lookup"><span data-stu-id="4c4b6-136">String</span></span>|<span data-ttu-id="4c4b6-137">カテゴリ名</span><span class="sxs-lookup"><span data-stu-id="4c4b6-137">The category name</span></span>|



## <a name="response"></a><span data-ttu-id="4c4b6-138">応答</span><span class="sxs-lookup"><span data-stu-id="4c4b6-138">Response</span></span>
<span data-ttu-id="4c4b6-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[Devicemanagementsettingcategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-139">If successful, this method returns a `200 OK` response code and an updated [deviceManagementSettingCategory](../resources/intune-deviceintent-devicemanagementsettingcategory.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="4c4b6-140">例</span><span class="sxs-lookup"><span data-stu-id="4c4b6-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="4c4b6-141">要求</span><span class="sxs-lookup"><span data-stu-id="4c4b6-141">Request</span></span>
<span data-ttu-id="4c4b6-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/deviceManagement/categories/{deviceManagementSettingCategoryId}
Content-type: application/json
Content-length: 113

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "displayName": "Display Name value"
}
```

### <a name="response"></a><span data-ttu-id="4c4b6-143">応答</span><span class="sxs-lookup"><span data-stu-id="4c4b6-143">Response</span></span>
<span data-ttu-id="4c4b6-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="4c4b6-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 162

{
  "@odata.type": "#microsoft.graph.deviceManagementSettingCategory",
  "id": "4f56472c-472c-4f56-2c47-564f2c47564f",
  "displayName": "Display Name value"
}
```




