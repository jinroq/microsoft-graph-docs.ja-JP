---
title: WindowsOfficeClientSecurityConfiguration の削除
description: セキュリティポリシー windowsOfficeClientSecurityConfiguration を削除します。
localization_priority: Normal
author: rolyon
ms.prod: Intune
ms.openlocfilehash: 400b8b9e1c8d83983f08eab2013a72be3178c73f
ms.sourcegitcommit: 94aaf594c881c02f353c6a417460cdf783a0bfe0
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 05/11/2019
ms.locfileid: "33933964"
---
# <a name="delete-windowsofficeclientsecurityconfiguration"></a><span data-ttu-id="73936-103">WindowsOfficeClientSecurityConfiguration の削除</span><span class="sxs-lookup"><span data-stu-id="73936-103">Delete windowsOfficeClientSecurityConfiguration</span></span>

> <span data-ttu-id="73936-104">**重要:** ベータ版の Microsoft Graph Api は変更される可能性があります。運用環境での使用はサポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73936-104">**Important:** Microsoft Graph APIs under the /beta version are subject to change; production use is not supported.</span></span>

> <span data-ttu-id="73936-105">**注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="73936-105">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="73936-106">セキュリティポリシー [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md)を削除します。</span><span class="sxs-lookup"><span data-stu-id="73936-106">Deletes a security policy [windowsOfficeClientSecurityConfiguration](../resources/intune-cirrus-windowsofficeclientsecurityconfiguration.md).</span></span>

## <a name="prerequisites"></a><span data-ttu-id="73936-107">前提条件</span><span class="sxs-lookup"><span data-stu-id="73936-107">Prerequisites</span></span>
<span data-ttu-id="73936-p101">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/graph/permissions-reference)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="73936-p101">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/graph/permissions-reference).</span></span>

|<span data-ttu-id="73936-110">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="73936-110">Permission type</span></span>|<span data-ttu-id="73936-111">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="73936-111">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="73936-112">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="73936-112">Delegated (work or school account)</span></span>|<span data-ttu-id="73936-113">DeviceManagementConfiguration.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="73936-113">DeviceManagementConfiguration.ReadWrite.All</span></span>|
|<span data-ttu-id="73936-114">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="73936-114">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="73936-115">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73936-115">Not supported.</span></span>|
|<span data-ttu-id="73936-116">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="73936-116">Application</span></span>|<span data-ttu-id="73936-117">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="73936-117">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="73936-118">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="73936-118">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
DELETE /officeConfiguration/clientConfigurations/{key}
```

## <a name="request-headers"></a><span data-ttu-id="73936-119">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73936-119">Request headers</span></span>
|<span data-ttu-id="73936-120">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="73936-120">Header</span></span>|<span data-ttu-id="73936-121">値</span><span class="sxs-lookup"><span data-stu-id="73936-121">Value</span></span>|
|:---|:---|
|<span data-ttu-id="73936-122">Authorization</span><span class="sxs-lookup"><span data-stu-id="73936-122">Authorization</span></span>|<span data-ttu-id="73936-123">ベアラー &lt;トークン&gt; が必要です。</span><span class="sxs-lookup"><span data-stu-id="73936-123">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="73936-124">承諾</span><span class="sxs-lookup"><span data-stu-id="73936-124">Accept</span></span>|<span data-ttu-id="73936-125">application/json</span><span class="sxs-lookup"><span data-stu-id="73936-125">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="73936-126">要求本文</span><span class="sxs-lookup"><span data-stu-id="73936-126">Request body</span></span>
<span data-ttu-id="73936-127">このメソッドには、要求本文を指定しません。</span><span class="sxs-lookup"><span data-stu-id="73936-127">Do not supply a request body for this method.</span></span>

## <a name="response"></a><span data-ttu-id="73936-128">応答</span><span class="sxs-lookup"><span data-stu-id="73936-128">Response</span></span>
<span data-ttu-id="73936-129">成功した場合、このメソッドは `200 OK` 応答コードを返します。</span><span class="sxs-lookup"><span data-stu-id="73936-129">If successful, this method returns a `200 OK` response code.</span></span>

## <a name="example"></a><span data-ttu-id="73936-130">例</span><span class="sxs-lookup"><span data-stu-id="73936-130">Example</span></span>

### <a name="request"></a><span data-ttu-id="73936-131">要求</span><span class="sxs-lookup"><span data-stu-id="73936-131">Request</span></span>
<span data-ttu-id="73936-132">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="73936-132">Here is an example of the request.</span></span>
``` http
DELETE https://graph.microsoft.com/beta/officeConfiguration/clientConfigurations/{key}
```

### <a name="response"></a><span data-ttu-id="73936-133">応答</span><span class="sxs-lookup"><span data-stu-id="73936-133">Response</span></span>
<span data-ttu-id="73936-p102">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="73936-p102">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 200 OK
```



