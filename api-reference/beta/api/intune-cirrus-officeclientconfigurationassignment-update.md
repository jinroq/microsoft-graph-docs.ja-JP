---
title: OfficeClientConfigurationAssignment の更新
description: OfficeClientConfigurationAssignment オブジェクトのプロパティを更新します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 80b748ddff1926d0f2794c7fc9d65cde05e5faa2
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33934041"
---
# <a name="update-officeclientconfigurationassignment"></a><span data-ttu-id="e38b7-103">OfficeClientConfigurationAssignment の更新</span><span class="sxs-lookup"><span data-stu-id="e38b7-103">Update officeClientConfigurationAssignment</span></span>

> <span data-ttu-id="e38b7-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38b7-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="e38b7-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="e38b7-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="e38b7-106">[OfficeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトのプロパティを更新します。</span><span class="sxs-lookup"><span data-stu-id="e38b7-106">Update the properties of a [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="e38b7-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="e38b7-107">Prerequisites</span></span>
<span data-ttu-id="e38b7-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="e38b7-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="e38b7-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="e38b7-110">Permission type</span></span>|<span data-ttu-id="e38b7-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="e38b7-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="e38b7-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="e38b7-112">Delegated (work or school account)</span></span>|<span data-ttu-id="e38b7-113">\* \* TODO: 範囲を決定します \* \*</span><span class="sxs-lookup"><span data-stu-id="e38b7-113">\*\*TODO: Determine scopes \*\*</span></span>|
|<span data-ttu-id="e38b7-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="e38b7-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="e38b7-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38b7-115">Not supported.</span></span>|
|<span data-ttu-id="e38b7-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="e38b7-116">Application</span></span>|<span data-ttu-id="e38b7-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="e38b7-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="e38b7-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="e38b7-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
PATCH /officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
```

## <a name="request-headers"></a><span data-ttu-id="e38b7-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38b7-119">Request headers</span></span>
|<span data-ttu-id="e38b7-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="e38b7-120">Header</span></span>|<span data-ttu-id="e38b7-121">値</span><span class="sxs-lookup"><span data-stu-id="e38b7-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="e38b7-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="e38b7-122">Authorization</span></span>|<span data-ttu-id="e38b7-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="e38b7-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="e38b7-124">承諾</span><span class="sxs-lookup"><span data-stu-id="e38b7-124">Accept</span></span>|<span data-ttu-id="e38b7-125">application/json</span><span class="sxs-lookup"><span data-stu-id="e38b7-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="e38b7-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="e38b7-126">Request body</span></span>
<span data-ttu-id="e38b7-127">要求本文で、 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトの JSON 表記を指定します。</span><span class="sxs-lookup"><span data-stu-id="e38b7-127">In the request body, supply a JSON representation for the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object.</span></span>

<span data-ttu-id="e38b7-128">次の表に、 [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)の作成時に必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="e38b7-128">The following table shows the properties that are required when you create the [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md).</span></span>

|<span data-ttu-id="e38b7-129">プロパティ</span><span class="sxs-lookup"><span data-stu-id="e38b7-129">Property</span></span>|<span data-ttu-id="e38b7-130">型</span><span class="sxs-lookup"><span data-stu-id="e38b7-130">Type</span></span>|<span data-ttu-id="e38b7-131">説明</span><span class="sxs-lookup"><span data-stu-id="e38b7-131">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="e38b7-132">id</span><span class="sxs-lookup"><span data-stu-id="e38b7-132">id</span></span>|<span data-ttu-id="e38b7-133">String</span><span class="sxs-lookup"><span data-stu-id="e38b7-133">String</span></span>|<span data-ttu-id="e38b7-134">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e38b7-134">Not yet documented</span></span>|
|<span data-ttu-id="e38b7-135">target</span><span class="sxs-lookup"><span data-stu-id="e38b7-135">target</span></span>|[<span data-ttu-id="e38b7-136">officeConfigurationAssignmentTarget</span><span class="sxs-lookup"><span data-stu-id="e38b7-136">officeConfigurationAssignmentTarget</span></span>](../resources/intune-cirrus-officeconfigurationassignmenttarget.md)|<span data-ttu-id="e38b7-137">まだ文書化されていません</span><span class="sxs-lookup"><span data-stu-id="e38b7-137">Not yet documented</span></span>|



## <a name="response"></a><span data-ttu-id="e38b7-138">応答</span><span class="sxs-lookup"><span data-stu-id="e38b7-138">Response</span></span>
<span data-ttu-id="e38b7-139">成功した場合、このメソッド`200 OK`は応答コードと、応答本文で更新された[officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md)オブジェクトを返します。</span><span class="sxs-lookup"><span data-stu-id="e38b7-139">If successful, this method returns a `200 OK` response code and an updated [officeClientConfigurationAssignment](../resources/intune-cirrus-officeclientconfigurationassignment.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="e38b7-140">例</span><span class="sxs-lookup"><span data-stu-id="e38b7-140">Example</span></span>

### <a name="request"></a><span data-ttu-id="e38b7-141">要求</span><span class="sxs-lookup"><span data-stu-id="e38b7-141">Request</span></span>
<span data-ttu-id="e38b7-142">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="e38b7-142">Here is an example of the request.</span></span>
``` http
PATCH https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{officeClientConfigurationId}/assignments/{officeClientConfigurationAssignmentId}
Content-type: application/json
Content-length: 98

{
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```

### <a name="response"></a><span data-ttu-id="e38b7-143">応答</span><span class="sxs-lookup"><span data-stu-id="e38b7-143">Response</span></span>
<span data-ttu-id="e38b7-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="e38b7-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
Content-Type: application/json
Content-Length: 221

{
  "@odata.type": "#microsoft.graph.officeClientConfigurationAssignment",
  "id": "804730f3-30f3-8047-f330-4780f3304780",
  "target": {
    "@odata.type": "microsoft.graph.officeConfigurationAssignmentTarget"
  }
}
```



