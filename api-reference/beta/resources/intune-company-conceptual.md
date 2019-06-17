---
title: Microsoft Intune での会社の使用条件-Microsoft Graph API
description: テナント組織の使用条件を定義する Intune エンドポイント (REST) の Microsoft Graph API を一覧表示します。
localization_priority: Normal
author: rolyon
ms.prod: intune
ms.openlocfilehash: c10487c6d708c3c8f7868abd07a629084b6447c2
ms.sourcegitcommit: 0a62bc5849f27a55d83efce9b3eb01b9711bbe1d
ms.translationtype: MT
ms.contentlocale: ja-JP
ms.lasthandoff: 06/14/2019
ms.locfileid: "34989505"
---
# <a name="company-terms-and-conditions-in-microsoft-intune"></a>Microsoft Intune の会社の使用条件

> **重要:** Microsoft Graph のベータ版 (/beta) の API はプレビュー中であるため、変更されることがあります。 実稼働アプリケーションでは、これらの API の使用はサポートされていません。

> **注:** Microsoft Graph API for Intune では、テナントに対して[アクティブな intune ライセンス](https://go.microsoft.com/fwlink/?linkid=839381)が必要です。

Intune の使用条件をユーザー グループに展開して、登録、作業リソースへのアクセス、ポータル サイト アプリがデバイスやユーザーにどのように影響するかを説明することができます。 ポータル サイトを使用して自分の仕事に登録してアクセスするには、ユーザーはまず使用条件に同意する必要があります。

さまざまな使用条件を含む複数のポリシーを作成して展開することができます。 同じ使用条件のバージョンを異なる言語で作成し、それぞれ適切なグループに展開することもできます。

次の Graph リソースを使用して、Intune での会社の使用条件を管理できます。

- [使用条件](intune-companyterms-termsandconditions.md)
- [使用条件の承認状態](intune-companyterms-termsandconditionsacceptancestatus.md)
- [使用条件の割り当て](intune-companyterms-termsandconditionsassignment.md)
- [条項および条件のグループの割り当て](intune-companyterms-termsandconditionsgroupassignment.md)
