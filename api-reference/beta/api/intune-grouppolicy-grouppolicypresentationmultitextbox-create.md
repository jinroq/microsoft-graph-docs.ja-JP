---
title: GroupPolicyPresentationMultiTextBox を作成します。
description: 新しい groupPolicyPresentationMultiTextBox オブジェクトを作成します。
localization_priority: Normal
author: tfitzmac
ms.prod: Intune
ms.openlocfilehash: 41042c5ad62cb56573e924c69b62cef72ee6835c
ms.sourcegitcommit: dcc5907f2c3ffc0f0e82e953b7ab9cf4ab938360
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 01/23/2019
ms.locfileid: "29430251"
---
# <a name="create-grouppolicypresentationmultitextbox"></a><span data-ttu-id="834a4-103">GroupPolicyPresentationMultiTextBox を作成します。</span><span class="sxs-lookup"><span data-stu-id="834a4-103">Create groupPolicyPresentationMultiTextBox</span></span>

> <span data-ttu-id="834a4-104">**重要な:**[Microsoft Graph で/beta のバージョンの Api は予告なしに変更されることがあります。</span><span class="sxs-lookup"><span data-stu-id="834a4-104">**Important:** APIs under the /beta version in Microsoft Graph are subject to change.</span></span> <span data-ttu-id="834a4-105">実稼働アプリケーションでこれらの API を使用することは、サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="834a4-105">Use of these APIs in production applications is not supported.</span></span>

> <span data-ttu-id="834a4-106">**注:** Intune の Microsoft グラフ API では、テナントの[Intune のアクティブなライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。</span><span class="sxs-lookup"><span data-stu-id="834a4-106">**Note:** The Microsoft Graph API for Intune requires an [active Intune license](https://go.microsoft.com/fwlink/?linkid=839381) for the tenant.</span></span>

<span data-ttu-id="834a4-107">新しい[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトを作成します。</span><span class="sxs-lookup"><span data-stu-id="834a4-107">Create a new [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object.</span></span>

## <a name="prerequisites"></a><span data-ttu-id="834a4-108">前提条件</span><span class="sxs-lookup"><span data-stu-id="834a4-108">Prerequisites</span></span>
<span data-ttu-id="834a4-p102">この API を呼び出すには、次のいずれかのアクセス許可が必要です。アクセス許可の選択方法などの詳細については、「[アクセス許可](/concepts/permissions-reference.md)」を参照してください。</span><span class="sxs-lookup"><span data-stu-id="834a4-p102">One of the following permissions is required to call this API. To learn more, including how to choose permissions, see [Permissions](/concepts/permissions-reference.md).</span></span>

|<span data-ttu-id="834a4-111">アクセス許可の種類</span><span class="sxs-lookup"><span data-stu-id="834a4-111">Permission type</span></span>|<span data-ttu-id="834a4-112">アクセス許可 (特権の大きいものから小さいものへ)</span><span class="sxs-lookup"><span data-stu-id="834a4-112">Permissions (from most to least privileged)</span></span>|
|:---|:---|
|<span data-ttu-id="834a4-113">委任 (職場または学校のアカウント)</span><span class="sxs-lookup"><span data-stu-id="834a4-113">Delegated (work or school account)</span></span>|<span data-ttu-id="834a4-114">DeviceManagementServiceConfig.ReadWrite.All</span><span class="sxs-lookup"><span data-stu-id="834a4-114">DeviceManagementServiceConfig.ReadWrite.All</span></span>|
|<span data-ttu-id="834a4-115">委任 (個人用 Microsoft アカウント)</span><span class="sxs-lookup"><span data-stu-id="834a4-115">Delegated (personal Microsoft account)</span></span>|<span data-ttu-id="834a4-116">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="834a4-116">Not supported.</span></span>|
|<span data-ttu-id="834a4-117">アプリケーション</span><span class="sxs-lookup"><span data-stu-id="834a4-117">Application</span></span>|<span data-ttu-id="834a4-118">サポートされていません。</span><span class="sxs-lookup"><span data-stu-id="834a4-118">Not supported.</span></span>|

## <a name="http-request"></a><span data-ttu-id="834a4-119">HTTP 要求</span><span class="sxs-lookup"><span data-stu-id="834a4-119">HTTP Request</span></span>
<!-- {
  "blockType": "ignored"
}
-->
``` http
POST /deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
```

## <a name="request-headers"></a><span data-ttu-id="834a4-120">要求ヘッダー</span><span class="sxs-lookup"><span data-stu-id="834a4-120">Request headers</span></span>
|<span data-ttu-id="834a4-121">ヘッダー</span><span class="sxs-lookup"><span data-stu-id="834a4-121">Header</span></span>|<span data-ttu-id="834a4-122">値</span><span class="sxs-lookup"><span data-stu-id="834a4-122">Value</span></span>|
|:---|:---|
|<span data-ttu-id="834a4-123">Authorization</span><span class="sxs-lookup"><span data-stu-id="834a4-123">Authorization</span></span>|<span data-ttu-id="834a4-124">ベアラー &lt;トークン&gt; が必須。</span><span class="sxs-lookup"><span data-stu-id="834a4-124">Bearer &lt;token&gt; Required.</span></span>|
|<span data-ttu-id="834a4-125">Accept</span><span class="sxs-lookup"><span data-stu-id="834a4-125">Accept</span></span>|<span data-ttu-id="834a4-126">application/json</span><span class="sxs-lookup"><span data-stu-id="834a4-126">application/json</span></span>|

## <a name="request-body"></a><span data-ttu-id="834a4-127">要求本文</span><span class="sxs-lookup"><span data-stu-id="834a4-127">Request body</span></span>
<span data-ttu-id="834a4-128">要求の本文に groupPolicyPresentationMultiTextBox オブジェクトの JSON の形式を指定します。</span><span class="sxs-lookup"><span data-stu-id="834a4-128">In the request body, supply a JSON representation for the groupPolicyPresentationMultiTextBox object.</span></span>

<span data-ttu-id="834a4-129">次の表は、groupPolicyPresentationMultiTextBox を作成するときに必要なプロパティを示します。</span><span class="sxs-lookup"><span data-stu-id="834a4-129">The following table shows the properties that are required when you create the groupPolicyPresentationMultiTextBox.</span></span>

|<span data-ttu-id="834a4-130">プロパティ</span><span class="sxs-lookup"><span data-stu-id="834a4-130">Property</span></span>|<span data-ttu-id="834a4-131">型</span><span class="sxs-lookup"><span data-stu-id="834a4-131">Type</span></span>|<span data-ttu-id="834a4-132">説明</span><span class="sxs-lookup"><span data-stu-id="834a4-132">Description</span></span>|
|:---|:---|:---|
|<span data-ttu-id="834a4-133">label</span><span class="sxs-lookup"><span data-stu-id="834a4-133">label</span></span>|<span data-ttu-id="834a4-134">String</span><span class="sxs-lookup"><span data-stu-id="834a4-134">String</span></span>|<span data-ttu-id="834a4-135">プレゼンテーションの任意のエンティティのローカライズされたテキスト ラベルです。</span><span class="sxs-lookup"><span data-stu-id="834a4-135">Localized text label for any presentation entity.</span></span> <span data-ttu-id="834a4-136">既定値は空です。</span><span class="sxs-lookup"><span data-stu-id="834a4-136">The default value is empty.</span></span> <span data-ttu-id="834a4-137">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="834a4-137">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="834a4-138">id</span><span class="sxs-lookup"><span data-stu-id="834a4-138">id</span></span>|<span data-ttu-id="834a4-139">String</span><span class="sxs-lookup"><span data-stu-id="834a4-139">String</span></span>|<span data-ttu-id="834a4-140">エンティティのキー。</span><span class="sxs-lookup"><span data-stu-id="834a4-140">Key of the entity.</span></span> <span data-ttu-id="834a4-141">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="834a4-141">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="834a4-142">lastModifiedDateTime</span><span class="sxs-lookup"><span data-stu-id="834a4-142">lastModifiedDateTime</span></span>|<span data-ttu-id="834a4-143">DateTimeOffset</span><span class="sxs-lookup"><span data-stu-id="834a4-143">DateTimeOffset</span></span>|<span data-ttu-id="834a4-144">日付と時刻、エンティティが最後に修正されました。</span><span class="sxs-lookup"><span data-stu-id="834a4-144">The date and time the entity was last modified.</span></span> <span data-ttu-id="834a4-145">[GroupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)から継承されました。</span><span class="sxs-lookup"><span data-stu-id="834a4-145">Inherited from [groupPolicyPresentation](../resources/intune-grouppolicy-grouppolicypresentation.md)</span></span>|
|<span data-ttu-id="834a4-146">必須</span><span class="sxs-lookup"><span data-stu-id="834a4-146">required</span></span>|<span data-ttu-id="834a4-147">Boolean</span><span class="sxs-lookup"><span data-stu-id="834a4-147">Boolean</span></span>|<span data-ttu-id="834a4-148">テキスト ボックスに値を入力するための要件。</span><span class="sxs-lookup"><span data-stu-id="834a4-148">Requirement to enter a value in the text box.</span></span> <span data-ttu-id="834a4-149">既定値は false です。</span><span class="sxs-lookup"><span data-stu-id="834a4-149">Default value is false.</span></span>|
|<span data-ttu-id="834a4-150">maxLength</span><span class="sxs-lookup"><span data-stu-id="834a4-150">maxLength</span></span>|<span data-ttu-id="834a4-151">Int64</span><span class="sxs-lookup"><span data-stu-id="834a4-151">Int64</span></span>|<span data-ttu-id="834a4-152">テキスト文字の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="834a4-152">An unsigned integer that specifies the maximum number of text characters.</span></span> <span data-ttu-id="834a4-153">1023 を既定値には。</span><span class="sxs-lookup"><span data-stu-id="834a4-153">Default value is 1023.</span></span>|
|<span data-ttu-id="834a4-154">maxStrings</span><span class="sxs-lookup"><span data-stu-id="834a4-154">maxStrings</span></span>|<span data-ttu-id="834a4-155">Int64</span><span class="sxs-lookup"><span data-stu-id="834a4-155">Int64</span></span>|<span data-ttu-id="834a4-156">文字列の最大数を指定する符号なし整数。</span><span class="sxs-lookup"><span data-stu-id="834a4-156">An unsigned integer that specifies the maximum number of strings.</span></span> <span data-ttu-id="834a4-157">既定値は 0 です。</span><span class="sxs-lookup"><span data-stu-id="834a4-157">Default value is 0.</span></span>|



## <a name="response"></a><span data-ttu-id="834a4-158">応答</span><span class="sxs-lookup"><span data-stu-id="834a4-158">Response</span></span>
<span data-ttu-id="834a4-159">かどうかは成功すると、このメソッドが返されます、`201 Created`応答コードおよび応答の本文に[groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md)オブジェクトです。</span><span class="sxs-lookup"><span data-stu-id="834a4-159">If successful, this method returns a `201 Created` response code and a [groupPolicyPresentationMultiTextBox](../resources/intune-grouppolicy-grouppolicypresentationmultitextbox.md) object in the response body.</span></span>

## <a name="example"></a><span data-ttu-id="834a4-160">例</span><span class="sxs-lookup"><span data-stu-id="834a4-160">Example</span></span>

### <a name="request"></a><span data-ttu-id="834a4-161">要求</span><span class="sxs-lookup"><span data-stu-id="834a4-161">Request</span></span>
<span data-ttu-id="834a4-162">以下は、要求の例です。</span><span class="sxs-lookup"><span data-stu-id="834a4-162">Here is an example of the request.</span></span>
``` http
POST https://graph.microsoft.com/beta/deviceManagement/groupPolicyConfigurations/{groupPolicyConfigurationId}/definitionValues/{groupPolicyDefinitionValueId}/presentationValues/{groupPolicyPresentationValueId}/presentation/definition/presentations
Content-type: application/json
Content-length: 165

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```

### <a name="response"></a><span data-ttu-id="834a4-163">応答</span><span class="sxs-lookup"><span data-stu-id="834a4-163">Response</span></span>
<span data-ttu-id="834a4-p109">以下は、応答の例です。注:簡潔にするために、ここに示す応答オブジェクトは切り詰められている場合があります。すべてのプロパティは実際の呼び出しから返されます。</span><span class="sxs-lookup"><span data-stu-id="834a4-p109">Here is an example of the response. Note: The response object shown here may be truncated for brevity. All of the properties will be returned from an actual call.</span></span>
``` http
HTTP/1.1 201 Created
Content-Type: application/json
Content-Length: 278

{
  "@odata.type": "#microsoft.graph.groupPolicyPresentationMultiTextBox",
  "label": "Label value",
  "id": "381ac035-c035-381a-35c0-1a3835c01a38",
  "lastModifiedDateTime": "2017-01-01T00:00:35.1329464-08:00",
  "required": true,
  "maxLength": 9,
  "maxStrings": 10
}
```




